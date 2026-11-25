# Tabla de BPM a ms para hard techno, de 140 a 220 BPM

> Milisegundos por negra, corchea, semicorchea y compás de 140 a 220 BPM, con las fórmulas y un ejemplo para calcular la duración en segundos.

- Web: https://apps.schimpf.es/tekkno-rave-daw/es/bpm-to-ms-chart/
- App: Tekkno Rave DAW: Crea Beats, https://apps.schimpf.es/tekkno-rave-daw/es/index.md
Los tiempos de delay, la longitud de los bucles y los cortes de muestras resultan más fáciles si sabes cuántos milisegundos dura un pulso. Esta página trae una tabla para el rango de tempo del hard techno y el hardcore (de 140 a 220 BPM), las fórmulas que hay detrás y una calculadora pequeña.

## Las fórmulas

BPM significa pulsos por minuto (beats per minute). Un minuto tiene 60 000 milisegundos, así que:

- Pulso (negra) en ms = 60000 / BPM
- Corchea en ms = 30000 / BPM
- Semicorchea en ms = 15000 / BPM
- Compás de 4/4 en ms = 240000 / BPM

Un compás de 4/4 tiene 4 pulsos, que son 16 semicorcheas. La mayoría de los secuenciadores por pasos, incluido un patrón de 16 pasos, tratan cada paso como una semicorchea.

## Tabla de BPM a ms

| BPM | Semicorchea (ms) | Corchea (ms) | Negra (ms) | Compás (ms) |
|-----|------------------|--------------|------------|-------------|
| 140 | 107,14 | 214,29 | 428,57 | 1714,29 |
| 150 | 100,00 | 200,00 | 400,00 | 1600,00 |
| 160 | 93,75 | 187,50 | 375,00 | 1500,00 |
| 170 | 88,24 | 176,47 | 352,94 | 1411,76 |
| 175 | 85,71 | 171,43 | 342,86 | 1371,43 |
| 180 | 83,33 | 166,67 | 333,33 | 1333,33 |
| 190 | 78,95 | 157,89 | 315,79 | 1263,16 |
| 200 | 75,00 | 150,00 | 300,00 | 1200,00 |
| 210 | 71,43 | 142,86 | 285,71 | 1142,86 |
| 220 | 68,18 | 136,36 | 272,73 | 1090,91 |

Los valores están redondeados a dos decimales.

## Ejemplo: ¿cuánto dura mi tema?

Supón que escribes un tema a 175 BPM de 32 compases.

1. Un compás a 175 BPM = 240000 / 175 = 1371,43 ms.
2. 32 compases = 32 x 1371,43 = 43 885,7 ms.
3. Son unos 43,9 segundos.

Puedes comprobarlo de otra forma. 32 compases x 16 pasos = 512 pasos. Un paso a 175 BPM = 15000 / 175 = 85,71 ms. 512 x 85,71 = 43 885,7 ms. El resultado es el mismo.

Los temas más largos crecen en línea recta: 64 compases a 175 BPM duran unos 87,8 segundos y 128 compases, unos 175,5 segundos.

## De milisegundos a frames de audio

El audio digital se cuenta en frames. Con una frecuencia de muestreo de 44,1 kHz hay 44 100 frames por segundo.

Frames por semicorchea = 44100 x 60 / BPM / 4

A 175 BPM son 44100 x 60 / 175 / 4 = 3780 frames por paso. Un tempo que divide de forma exacta como este mantiene los pasos en frames enteros. A 170 BPM el resultado es 3891,18 frames, así que el secuenciador tiene que llevar una posición con decimales para no desajustarse en un bucle largo.

## ¿Qué tempo para qué estilo?

Los rangos de tempo son convenciones flexibles. Los nombres de género se solapan y los productores se salen de los rangos continuamente. Como guía aproximada:

- El hard techno suele estar entre 150 y 160 BPM.
- El gabber y el hardcore suelen estar entre 170 y 200 BPM.
- El speedcore va aún más rápido.

La tabla de arriba cubre de 140 a 220 BPM, el rango del control de tempo de la app.

## Consejos para usar los números

- Para un tiempo de delay que caiga en la cuadrícula, usa el valor de la corchea o de la semicorchea de la tabla. Una corchea con puntillo es 1,5 veces el valor de la corchea.
- Un bombo en cada pulso a 175 BPM se repite cada 342,86 ms. Son 175 bombos por minuto.
- Un tempo más rápido acorta cada paso. Las muestras que suenan más que un paso se solapan con el siguiente golpe, así que recorta las colas de bombos y bajos largos cuando subas los BPM.
- En un secuenciador por pasos, cambiar el tempo no cambia el tono. Solo cambia la separación entre disparos.

## Calculadora

An interactive calculator is on the web page: https://apps.schimpf.es/tekkno-rave-daw/es/bpm-to-ms-chart/

## Pruébalo en la app

Tekkno Rave DAW es una groovebox para Android de hard techno y hardcore. Su control de tempo va de 140 a 220 BPM, un patrón tiene 8, 16, 32 o 64 pasos y un paso es una semicorchea. En la vista de canción un compás son 16 pasos, así que la fórmula de duración de arriba es la que usa la app al reproducir.
