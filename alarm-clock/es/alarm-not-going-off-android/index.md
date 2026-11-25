# La alarma no suena en Android: causas y soluciones

> Por qué la alarma de Android no suena o llega tarde, y una lista de ajustes para arreglarlo: alarmas exactas, notificaciones y batería.

- Web: https://apps.schimpf.es/alarm-clock/es/alarm-not-going-off-android/
- App: Despertador con misiones, https://apps.schimpf.es/alarm-clock/es/index.md
Una alarma que no suena suele estar bloqueada por un ajuste. Esta página enumera las causas más comunes en Android y cómo comprobar cada una.

## Lista rápida

1. La alarma está activada y los días correctos están seleccionados.
2. La hora es correcta (comprueba la mañana y la tarde, por ejemplo 6:30 y 18:30).
3. El volumen de la alarma está alto (no el volumen multimedia).
4. Las notificaciones de la app de alarma están permitidas.
5. El permiso de alarmas exactas está concedido, si tu versión de Android lo pide.
6. La optimización de batería no restringe la app.
7. Los límites en segundo plano del fabricante de tu teléfono no detienen la app.
8. Has probado la alarma con una hora un minuto más tarde.

## Causa 1: El volumen de la alarma está bajo

Android tiene volúmenes separados para multimedia, tono de llamada y alarmas. Bajar el volumen multimedia no cambia el volumen de la alarma. Abre el panel de volumen, despliégalo y comprueba el control de la alarma. Despertador suena por el canal de alarma, así que suena incluso en modo silencio. Además sube el volumen poco a poco durante un tiempo que tú fijas, de 0 a 120 segundos (por defecto, 30). Con una subida larga, los primeros segundos suenan bajos a propósito. Pon 0 para empezar a volumen máximo.

## Causa 2: Permiso de alarmas exactas

Android 12 y 12L (API 31 y 32) pueden impedir que las apps programen alarmas exactas hasta que lo permitas. Android 13 y posteriores lo conceden automáticamente a las apps que son despertadores. Consulta *Schedule alarms* en la documentación de Android Developers. Si usas Android 12 o 12L, abre los accesos especiales de la app y permite alarmas y recordatorios.

## Causa 3: Las notificaciones están desactivadas

Si las notificaciones están bloqueadas, puede que la pantalla de la alarma no aparezca. Abre los ajustes de notificaciones de la app y actívalas. En Android 13 y posteriores, la app también debe pedir el permiso de notificaciones.

## Causa 4: Avisos a pantalla completa

En Android 14 y posteriores, una app necesita el permiso de notificaciones a pantalla completa para mostrar la pantalla de la alarma sobre la pantalla de bloqueo. Las apps de alarma cumplen los requisitos. Comprueba el permiso en los ajustes de la app si la pantalla sigue apagada cuando suena la alarma.

## Causa 5: Optimización de batería

Android ahorra energía limitando las apps que se ejecutan en segundo plano. Si excluyes tu app de alarma de la optimización de batería, baja el riesgo de que el sistema la retrase o la detenga. Abre los ajustes de batería de la app y elige la opción sin restricciones.

## Causa 6: Ahorro de batería de los fabricantes

Algunos fabricantes añaden sus propios límites encima de Android. Xiaomi, Redmi, Poco, Samsung, Huawei, Honor, OnePlus, Oppo, Vivo y Realme son los habituales. Pueden cerrar las apps que deslizas fuera de recientes o ponerlas a dormir. La web comunitaria *Don't kill my app* (dontkillmyapp.com) recoge lo que hace cada fabricante. La guía de configuración de Despertador incluye pasos para estas marcas.

## Causa 7: Reinicios y cambios de hora

Una alarma debe programarse de nuevo tras un reinicio, tras un cambio de hora y tras un cambio de zona horaria. Despertador lo hace solo. Si usas otra app, ábrela una vez tras una actualización o un reinicio y comprueba que la próxima alarma sigue apareciendo.

## Probar la alarma

No esperes a mañana para descubrirlo. Programa una alarma de prueba para un minuto más tarde y bloquea la pantalla. Si suena y la pantalla se enciende, los ajustes funcionan.

## Cómo ayuda Despertador

- Un asistente de configuración en el primer arranque recorre los ajustes de alarmas exactas, notificaciones, pantalla completa y batería, y muestra pasos específicos de cada marca.
- Una alarma de prueba suena un minuto después.
- Puedes volver a abrir el asistente desde Ajustes cuando quieras.
- La alarma se programa con la API de despertador del sistema, que Android trata como una alarma visible para el usuario.
- Si mueves o borras tu propio archivo de sonido, suena un tono incluido en lugar del silencio.
- Si sales de una misión para despertar, la alarma vuelve a sonar al cabo de un minuto, y también tras un reinicio si estaba sonando.

Despertador no tiene permiso de internet, ni cuenta, ni analíticas. Es de código abierto bajo la licencia GNU GPL v3 o posterior. La app está en inglés y alemán. Abre la app, termina el asistente de configuración una vez y ejecuta la prueba.
