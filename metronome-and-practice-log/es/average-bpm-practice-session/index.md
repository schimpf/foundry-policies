# Cómo calcular el BPM medio de una sesión de práctica

> Calcula el tempo medio ponderado por tiempo de una sesión cuando cambias el metrónomo, con un ejemplo paso a paso y errores comunes.

- Web: https://apps.schimpf.es/metronome-and-practice-log/es/average-bpm-practice-session/
- App: Metrónomo y Diario de Práctica, https://apps.schimpf.es/metronome-and-practice-log/es/index.md
Si cambias el tempo del metrónomo mientras practicas, te conviene un solo número para toda la sesión: el BPM medio. La media simple de los tempos que usaste da un resultado erróneo. Necesitas una media ponderada por tiempo.

## La fórmula

**BPM medio = (BPM1 x tiempo1 + BPM2 x tiempo2 + ...) / (tiempo1 + tiempo2 + ...)**

Cada tempo cuenta en proporción al tiempo que te quedaste en él. Usa la misma unidad de tiempo para todas las partes. Valen minutos o segundos.

Metrónomo y Diario de Práctica usa esta fórmula. Mientras tocas, la app suma el tempo multiplicado por el tiempo transcurrido y, al pausar, divide por el tiempo total.

## Ejemplo resuelto

Practicas una obra durante 20 minutos:

1. 10 minutos a 80 BPM.
2. 5 minutos a 100 BPM.
3. 5 minutos a 120 BPM.

Paso a paso:

1. Multiplica cada tempo por su tiempo: 80 x 10 = 800, 100 x 5 = 500, 120 x 5 = 600.
2. Suma los resultados: 800 + 500 + 600 = 1900.
3. Suma los tiempos: 10 + 5 + 5 = 20 minutos.
4. Divide: 1900 / 20 = 95 BPM.

```
80 BPM  |##########  10 min
100 BPM |#####        5 min
120 BPM |#####        5 min
Media: 95 BPM
```

La media simple de 80, 100 y 120 es 100. Es demasiado alta, porque pasaste la mitad de la sesión en el tempo más lento.

## BPM medio y último BPM son distintos

Una sesión tiene dos números de tempo que conviene guardar:

- El último BPM es el tempo al que paraste. En el ejemplo es 120.
- El BPM medio es la cifra ponderada por tiempo. En el ejemplo es 95.

El último BPM muestra dónde terminaste. El BPM medio muestra cómo trabajaste. Si calientas despacio y acabas rápido, el último BPM parece alto, mientras que la media abarca toda la sesión. Metrónomo y Diario de Práctica guarda los dos valores de cada sesión.

## Un segundo ejemplo con segundos

Tocas 45 segundos a 60 BPM y luego 15 segundos a 90 BPM.

1. 60 x 45 = 2700.
2. 90 x 15 = 1350.
3. Total: 4050, dividido entre 60 segundos = 67,5 BPM.

## Errores comunes

- Hacer la media de los tempos sin ponderar. Pondera siempre por tiempo.
- Contar las pausas. El tiempo con el metrónomo parado no entra en el cálculo. La app empieza una sesión al pulsar play y la termina al pausar, así que solo cuenta el tiempo de juego.
- Mezclar unidades. No uses minutos para una parte y segundos para otra.
- Esperar mucho de un cambio de tempo tardío. Un cambio cerca del final apenas mueve la media, y es lo correcto.

## Usar el BPM medio para seguir tu progreso

Una sesión dice poco, así que registra la misma obra durante varias semanas y observa cómo sube la media:

| Semana | BPM medio |
|---|---|
| 1 | 72 |
| 2 | 80 |
| 3 | 88 |
| 4 | 96 |

Unos 8 BPM más por semana son una tendencia clara. Si el número se estanca, mantén el tempo unos días más antes de avanzar.

## Qué registra la app

- Una sesión empieza al pulsar play y termina al pausar.
- Las sesiones de menos de 30 segundos se ignoran, así que una prueba rápida de tempo no ensucia el registro.
- Cada sesión guarda su obra (o "General"), el compás, el último tempo y el tempo medio ponderado por tiempo.
- Puedes editar o eliminar cualquier sesión, con deshacer.
- Cada día con al menos un minuto de práctica cuenta para tu racha diaria.
- Los gráficos de progreso de tempo por obra y la vista de 12 semanas forman parte de la compra de Pro. El gráfico de 7 días funciona sin ella.

Todos los datos se quedan en tu dispositivo. La app no tiene permiso de Internet ni cuenta.

## Pruébalo en la app

Metrónomo y Diario de Práctica es un metrónomo para Android que registra tu práctica automáticamente, así que no tienes que hacer estas cuentas a mano. Búscalo en Google Play.
