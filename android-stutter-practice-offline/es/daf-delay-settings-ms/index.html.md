# Retardo DAF en ms: qué valor elegir y por qué

> Qué retardo usar en la retroalimentación auditiva retardada (DAF) para tartamudez, la latencia del móvil, la fórmula y un ejemplo con calculadora.

- Web: https://apps.schimpf.es/android-stutter-practice-offline/es/daf-delay-settings-ms/
- App: Tartamudez: práctica con DAF, https://apps.schimpf.es/android-stutter-practice-offline/es/index.md
La retroalimentación auditiva retardada (DAF) reproduce tu propia voz una fracción de segundo tarde. El ajuste es un retardo en milisegundos (ms). En un móvil, el propio camino del audio ya añade retardo, así que el número que eliges no siempre es el retardo que oyes. Esta página muestra la fórmula y dos ejemplos resueltos.

## Qué es la DAF

Hablas al micrófono y la app reproduce tu voz en los auriculares tras un breve retardo. La DAF es una técnica de la terapia del habla para la tartamudez. Cuánto ayuda varía de una persona a otra, y el ajuste adecuado se encuentra mejor con un logopeda. Esta página es información general y no un consejo médico.

## Valores de retardo habituales

Stutter Practice te deja ajustar el retardo de 25 a 250 ms. Empieza en 75 ms y ofrece cuatro valores rápidos:

| Valor rápido | Retardo |
|---|---|
| 1 | 50 ms |
| 2 | 75 ms (también el valor inicial) |
| 3 | 100 ms |
| 4 | 150 ms |

Cambia el valor en pasos pequeños y quédate con el que te resulte cómodo.

## Por qué el móvil añade retardo

Todo móvil Android tiene algo de retardo entre el micrófono y los auriculares. Viene del búfer de entrada, del procesado y del búfer de salida, y se llama latencia del dispositivo. Si ajustas 100 ms en una app que la ignora, puedes oír 100 ms más la latencia del dispositivo.

Stutter Practice lee la latencia del dispositivo en una breve calibración y te deja afinarla pulsando al ritmo de unos clics. El valor guardado es:

- Latencia del dispositivo = latencia base medida + ajuste fino
- El ajuste fino es la mediana del retraso de tus últimas pulsaciones, entre 0 y 60 ms.

## La fórmula

- Retardo que añade la app = retardo objetivo − latencia del dispositivo
- Nunca baja de cero.
- Si el objetivo es menor que la latencia del dispositivo, oyes solo la latencia del dispositivo y la app muestra un aviso.

## Ejemplos resueltos

Supón que la calibración dio una latencia del dispositivo de 40 ms.

1. Quieres 100 ms. La app añade 100 − 40 = 60 ms. Oyes unos 100 ms en total.
2. Quieres 75 ms. La app añade 75 − 40 = 35 ms.
3. Quieres 25 ms. 25 − 40 es negativo, así que la app añade 0 ms. Oyes unos 40 ms, más de lo que pediste. La app te avisa de que tu ajuste está por debajo del retardo del dispositivo.

Ahora supón una latencia del dispositivo de 70 ms, algo habitual en algunos móviles:

| Objetivo | Añadido por la app | Oído (aprox.) |
|---|---|---|
| 50 ms | 0 ms | 70 ms |
| 75 ms | 5 ms | 75 ms |
| 100 ms | 30 ms | 100 ms |
| 150 ms | 80 ms | 150 ms |

## Pruébalo

An interactive calculator is on the web page: https://apps.schimpf.es/android-stutter-practice-offline/es/daf-delay-settings-ms/

## Los auriculares importan

- Usa auriculares con cable o USB. Añaden el menor retardo y lo mantienen estable.
- El Bluetooth añade un retardo extra que cambia de un dispositivo a otro, por eso la app muestra un aviso cuando hay una salida Bluetooth activa.
- El altavoz del móvil también se señala, porque añade retardo extra.
- La calibración se guarda para la salida que usaste. Si cambias de auriculares, calibra de nuevo.

## Practica con Stutter Practice

Stutter Practice es una app Android para DAF, habla con ritmo y ejercicios de inicio suave. Funciona sin conexión a internet, no tiene permiso de red y procesa tu voz en directo sin grabarla. Puedes cambiar el retardo con el control deslizante, los botones de más y menos o los valores rápidos mientras la DAF está activa. También puedes combinar la DAF con los textos de lectura en voz alta.
