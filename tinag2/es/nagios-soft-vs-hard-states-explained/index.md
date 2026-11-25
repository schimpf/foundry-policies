# Estados soft y hard en Nagios e Icinga explicados

> Qué significan los estados soft y hard en Nagios e Icinga 2, cómo cuentan los intentos de comprobación y cuánto tarda un fallo en ser hard.

- Web: https://apps.schimpf.es/tinag2/es/nagios-soft-vs-hard-states-explained/
- App: Tinag2: Alertas Icinga/Nagios, https://apps.schimpf.es/tinag2/es/index.md
Un servicio en Nagios, Naemon o Icinga 2 no avisa en la primera comprobación fallida. Primero pasa por un estado soft (blando) y solo se vuelve hard (duro) tras varias comprobaciones fallidas seguidas. Esta página explica los estados, el contador de intentos y los tiempos, con un ejemplo resuelto.

## Los cuatro estados de un servicio

Todo plugin de comprobación termina con un código de salida. El núcleo de monitorización lo convierte en un estado. Esto sigue las Nagios Plugin Development Guidelines (nagios-plugins.org) y la documentación de Icinga 2, capítulo "Monitoring Basics".

| Código de salida | Estado | Significado |
|---|---|---|
| 0 | OK | La comprobación fue correcta. |
| 1 | WARNING | El valor está fuera del umbral de aviso. |
| 2 | CRITICAL | El valor está fuera del umbral crítico, o el servicio está fallando. |
| 3 | UNKNOWN | El plugin no pudo decidir, por ejemplo por un argumento incorrecto o un timeout. |

Los hosts son más sencillos. Un host está UP o DOWN. Thruk también informa de UNREACHABLE: un host al que no se llega porque algo entre el servidor de monitorización y el host está caído.

## Tipos de estado soft y hard

El tipo de estado indica lo seguro que está el núcleo del problema.

- **Soft**: una comprobación falló, pero el número de fallos sigue por debajo de `max_check_attempts`. El núcleo sigue comprobando, ahora con el intervalo de reintento, que es más corto.
- **Hard**: los fallos llegaron a `max_check_attempts`, o el estado pasó de un estado de problema hard a otro. Normalmente las notificaciones se envían a partir de aquí.

Un estado soft que vuelve a OK antes del último intento nunca llega a hard. Esto filtra fallos breves, como un paquete perdido.

## Los tres ajustes que fijan los tiempos

Cada host y cada servicio tiene estos ajustes en su configuración:

1. `check_interval`: tiempo entre comprobaciones mientras el estado es estable.
2. `retry_interval`: tiempo entre comprobaciones mientras el estado es soft.
3. `max_check_attempts`: cuántas comprobaciones fallidas seguidas vuelven hard el estado. La primera comprobación fallida cuenta como intento 1.

## Cuánto tarda un fallo en ser hard

Contando desde la primera comprobación fallida:

tiempo hasta hard = (`max_check_attempts` − 1) × `retry_interval`

Contando desde el momento en que el servicio se rompió de verdad, el peor caso suma un intervalo de comprobación completo, porque el fallo puede empezar justo después de una comprobación correcta:

peor caso = `check_interval` + (`max_check_attempts` − 1) × `retry_interval`

## Ejemplo resuelto

Ajustes: `check_interval` de 5 minutos, `retry_interval` de 1 minuto, `max_check_attempts` de 3.

1. 09:55:00. La comprobación es correcta. Estado OK.
2. 09:55:30. El servicio se rompe. Todavía nadie se entera.
3. 10:00:00. La comprobación falla. Estado CRITICAL, soft, intento 1/3.
4. 10:01:00. La comprobación falla. CRITICAL, soft, intento 2/3.
5. 10:02:00. La comprobación falla. CRITICAL, hard, intento 3/3. Empiezan las notificaciones.

El estado pasó a hard 2 minutos después de la primera comprobación fallida: (3 − 1) × 1 minuto. Pasó a hard 6,5 minutos después de que el servicio se rompiera de verdad. El peor caso con estos ajustes es 5 + 2 = 7 minutos.

```
peor caso: 5 min (intervalo de comprobación) + 2 x 1 min (reintentos) = 7 min
           |#####|##|
```

Si la comprobación de las 10:01:00 hubiera sido correcta, el servicio habría vuelto a OK sin llegar nunca a hard, y nadie habría recibido una notificación.

## Ajustar los números

- Subir `max_check_attempts` elimina más falsas alarmas, pero retrasa las reales.
- Un `retry_interval` más corto adelanta el estado hard sin añadir ruido al ritmo de comprobación del estado estable.
- Para un servicio muy importante, un `max_check_attempts` bajo, como 2, junto con un intervalo de reintento corto mantiene el retraso pequeño.

## Un detalle de Icinga 2

Icinga 2 reinicia su contador interno `check_attempt` a 1 cuando un estado pasa a hard. Si lees el valor en bruto de la API en un problema hard, puede aparecer 1/3 en lugar de 3/3. Tinag2 muestra los problemas hard como máx/máx, igual que Nagios.

## Estados soft y hard en Tinag2

Tinag2 es un cliente Android para Icinga 2 y para Nagios/Naemon a través de Thruk. Lee del servidor el tipo de estado y el contador de intentos y los usa en tres sitios:

- **Detalle del problema** muestra el tipo de estado y los intentos, por ejemplo "soft 2/3" o "hard 3/3".
- **Hard only** es un filtro de la pantalla Problems que oculta los problemas soft.
- **Reglas de alertas** omiten por defecto los estados soft, así que solo te avisan de problemas hard. Puedes desactivarlo en la pantalla Alerts. También hay una opción para esperar 5 minutos antes de alertar, contados desde el último cambio de estado del problema, que atenúa las comprobaciones que cambian de un estado a otro sin parar.

La aplicación consulta el servidor cada 15 minutos en segundo plano y cuando deslizas para actualizar. Un problema hard llega a tu móvil en la siguiente sincronización después de volverse hard, no en el segundo exacto.

Tinag2 solo lee los problemas y actúa sobre ellos. No cambia los intervalos de comprobación ni el número de intentos; eso se hace en tu configuración de Icinga o Nagios.

Tinag2 te permite filtrar, buscar y reconocer problemas hard desde el móvil, y envía alertas solo de los problemas que te importan. Añade tu servidor Icinga 2 o Thruk en la aplicación para probarlo.
