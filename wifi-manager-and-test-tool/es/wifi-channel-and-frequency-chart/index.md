# Canales WiFi y frecuencias: tabla (2,4, 5 y 6 GHz)

> Convierte una frecuencia WiFi en MHz a su número de canal, con tabla para 2,4, 5 y 6 GHz y consejos para elegir el mejor canal.

- Web: https://apps.schimpf.es/wifi-manager-and-test-tool/es/wifi-channel-and-frequency-chart/
- App: Escáner WiFi y herramientas, https://apps.schimpf.es/wifi-manager-and-test-tool/es/index.md
Cada canal WiFi es un número que representa una frecuencia central en MHz. Esta página ofrece la tabla, las fórmulas con ejemplos y un conversor, y después explica cómo elegir un canal.

## Fórmulas

El número de canal sale de la frecuencia central (f, en MHz). La separación es de 5 MHz en las tres bandas. Son las mismas fórmulas que usa la app Escáner WiFi y herramientas.

| Banda | Rango de frecuencia (MHz) | Canal |
|---|---|---|
| 2,4 GHz | 2412 a 2472 | (f - 2407) / 5 |
| 2,4 GHz | 2484 | 14 |
| 5 GHz | 5160 a 5885 | (f - 5000) / 5 |
| 6 GHz | 5955 a 7115 | (f - 5950) / 5 |

El plan de canales está definido en IEEE Std 802.11 (la revisión de 2020 y sus enmiendas). Los canales que puedes usar dependen del país.

### Ejemplos

1. 2437 MHz: (2437 - 2407) / 5 = 30 / 5 = canal 6, 2,4 GHz.
2. 5180 MHz: (5180 - 5000) / 5 = 180 / 5 = canal 36, 5 GHz.
3. 5955 MHz: (5955 - 5950) / 5 = 5 / 5 = canal 1, 6 GHz. Los números de canal se repiten en 6 GHz, así que indica siempre la banda.
4. 2484 MHz es un caso especial: canal 14. Solo está permitido en Japón, y solo para el antiguo 802.11b.

## Convierte una frecuencia

An interactive calculator is on the web page: https://apps.schimpf.es/wifi-manager-and-test-tool/es/wifi-channel-and-frequency-chart/

## Tabla de canales de 2,4 GHz

| Canal | Frecuencia central (MHz) |
|---|---|
| 1 | 2412 |
| 2 | 2417 |
| 3 | 2422 |
| 4 | 2427 |
| 5 | 2432 |
| 6 | 2437 |
| 7 | 2442 |
| 8 | 2447 |
| 9 | 2452 |
| 10 | 2457 |
| 11 | 2462 |
| 12 | 2467 |
| 13 | 2472 |
| 14 | 2484 |

En Estados Unidos se permiten los canales 1 a 11. En España y en la mayor parte de Europa se permiten los canales 1 a 13.

## Ejemplos de 5 GHz

| Canal | Frecuencia central (MHz) |
|---|---|
| 36 | 5180 |
| 40 | 5200 |
| 44 | 5220 |
| 48 | 5240 |
| 100 | 5500 |
| 149 | 5745 |
| 165 | 5825 |

Algunos canales de 5 GHz (aproximadamente del 52 al 144) comparten espectro con radares. Tu router puede tener que cambiar de canal, y la conexión puede cortarse un momento.

## Ejemplos de 6 GHz

| Canal | Frecuencia central (MHz) |
|---|---|
| 1 | 5955 |
| 5 | 5975 |
| 37 | 6135 |
| 93 | 6415 |

La banda de 6 GHz la usan los dispositivos WiFi 6E y WiFi 7.

## ¿Qué canal debo usar?

- En 2,4 GHz cada canal ocupa 20 MHz, pero los canales están separados solo 5 MHz. Los vecinos en los canales 1 y 3 se solapan. Los únicos tres canales que no se solapan entre sí son el 1, el 6 y el 11. Usa uno de ellos.
- 5 GHz y 6 GHz tienen muchos más canales sin solapamiento, así que la saturación es un problema menor.
- Elige el canal que menos usen tus vecinos. Un router en modo "automático" suele hacerlo, aunque no siempre bien.
- Un canal más ancho (40, 80 o 160 MHz) da más velocidad, pero ocupa más espacio y sufre más interferencias.
- Si un dispositivo no ve tu red de 5 GHz, comprueba que tu router use un canal que el dispositivo admita.

## Encuentra tu canal en Android

La pantalla WiFi info de Escáner WiFi y herramientas muestra tu banda, canal y velocidad de enlace, y el estándar WiFi (WiFi 4, 5, 6 o 7) de tu conexión actual. La app calcula el canal con las fórmulas de arriba a partir de la frecuencia que informa Android. Android exige el permiso de ubicación para que una app lea el nombre de la red. La app no usa ni guarda tu ubicación.

Combínalo con la [tabla de intensidad de señal WiFi](wifi-signal-strength-chart) para ver si el problema es el canal o el nivel de señal.
