# Tabla de intensidad de señal WiFi (dBm y calidad)

> Qué significan los valores dBm del WiFi, de -30 a -100 dBm. Tabla, consulta rápida y qué hacer cuando la señal es débil.

- Web: https://apps.schimpf.es/wifi-manager-and-test-tool/es/wifi-signal-strength-chart/
- App: Escáner WiFi y herramientas, https://apps.schimpf.es/wifi-manager-and-test-tool/es/index.md
La intensidad de la señal WiFi se expresa como RSSI en dBm. El número es negativo, y cuanto más cerca de cero, más fuerte es la señal. Esta página ofrece una tabla, una pequeña herramienta de consulta y varias soluciones.

## Tabla de intensidad de señal WiFi

| Señal (dBm) | Calidad | Barras (de 4) | Qué esperar |
|---|---|---|---|
| -55 o más | Excelente | 4 | Velocidad completa. Las videollamadas y el streaming son estables. |
| -56 a -67 | Buena | 3 | Fiable para streaming, llamadas y navegación. |
| -68 a -75 | Aceptable | 2 | Funciona, pero baja la velocidad y las llamadas pueden entrecortarse. |
| -76 a -99 | Débil | 1 | Páginas lentas, cortes y retrasos largos. |
| -100 o menos | Sin señal | 0 | No se puede usar. |

Estos tramos son los que usa la app Escáner WiFi y herramientas. Otras herramientas trazan los límites unos dBm más arriba o abajo, así que tómalos como orientación.

## Cómo leer los dBm

- Los dBm son una escala logarítmica. Cada cambio de 3 dBm duplica o reduce a la mitad la potencia, aproximadamente.
- -50 dBm tiene unas 1000 veces más potencia que -80 dBm. Una caída de -55 a -75 es una pérdida de 100 veces.
- Un cambio de 1 o 2 dBm es ruido. La señal se mueve tanto cuando giras el cuerpo o mueves el teléfono.
- El valor es lo que recibe tu teléfono del router. No dice nada sobre lo bien que tu router oye a tu teléfono.

### Ejemplo

Mides -62 dBm en el salón y -79 dBm en el dormitorio.

1. Salón: -62 está entre -56 y -67, así que Buena.
2. Dormitorio: -79 está entre -76 y -99, así que Débil.
3. La diferencia es de 17 dBm, unas 50 veces menos potencia en el dormitorio (17 / 10 = 1,7, y 10^1,7 es aproximadamente 50).

Arregla primero el dormitorio.

## Comprueba un valor

An interactive calculator is on the web page: https://apps.schimpf.es/wifi-manager-and-test-tool/es/wifi-signal-strength-chart/

## Qué reduce tu señal

- Distancia. La señal cae rápido en los primeros metros y luego más despacio.
- Paredes. El ladrillo, el hormigón y la piedra restan más que el pladur. El metal y los espejos restan más que nada.
- Banda. 5 GHz y 6 GHz llegan menos lejos que 2,4 GHz y las paredes los bloquean más.
- Interferencias. Las redes vecinas en el mismo canal, los microondas y los teléfonos inalámbricos añaden ruido. Consulta la [tabla de canales WiFi](wifi-channel-and-frequency-chart) para encontrar un canal más tranquilo.
- Posición del router. Un router en el suelo, dentro de un mueble o en una esquina cubre menos de la casa.

## Cómo mejorar una señal débil

1. Mueve el router a un punto central, más alto y despejado.
2. Ve a la habitación con poca señal y mira el valor en directo mientras mueves el router o el teléfono.
3. Cambia a un canal menos saturado.
4. En 2,4 GHz, usa el canal 1, 6 u 11 para no solaparte con los vecinos más de lo necesario.
5. Si una habitación sigue floja, añade un punto de acceso o un nodo mesh a mitad de camino, conectado por cable si es posible.

## Mídela en tu teléfono

La pantalla WiFi info de Escáner WiFi y herramientas muestra tu señal actual en dBm con el nombre de la calidad y el medidor de cuatro barras de la tabla de arriba. También muestra banda, canal, velocidad de enlace y estándar WiFi. Android exige el permiso de ubicación para que una app pueda leer el nombre de la red. La app no usa ni guarda tu ubicación.

Recorre la casa con la pantalla abierta y anota el valor en cada habitación. Todo se queda en tu teléfono.

## Señal y velocidad

Hace falta una señal fuerte para tener velocidad, pero son dos valores distintos. La velocidad de enlace depende del estándar WiFi, del ancho del canal y de cuántos dispositivos comparten el canal. Una señal de -50 dBm en un canal saturado puede ser lenta. Si la señal es buena y la conexión sigue lenta, revisa el canal y haz un ping para ver la latencia.
