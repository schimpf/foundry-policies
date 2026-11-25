# Sección de cable a 12 V y caída de tensión, con ejemplo

> Cómo calcular la sección del cable en 12 V y 24 V. Fórmula de caída de tensión, ejemplo resuelto y longitud máxima por sección.

- Web: https://apps.schimpf.es/offline-wire-gauge-calculator/es/12v-wire-size-voltage-drop/
- App: Calculadora de cable: NEC, https://apps.schimpf.es/offline-wire-gauge-calculator/es/index.md
A 12 V, una pérdida pequeña de tensión pesa mucho. Una caída de 0,6 V es el 5 % a 12 V y solo el 0,25 % a 240 V. Por eso los tendidos de 12 V y 24 V (autocaravana, camper, barco, placas solares) se dimensionan primero por caída de tensión y después se comprueba la intensidad admisible (ampacidad). Esta página muestra la fórmula, un ejemplo resuelto y una tabla de longitudes máximas.

## La fórmula de caída de tensión en corriente continua

La corriente sale por un conductor y vuelve por el otro. Por eso cuenta la resistencia del doble de la longitud de ida.

1. Caída en voltios: caída = 2 × L × I × R
2. Caída en porcentaje: caída / tensión de alimentación × 100
3. Caída permitida en voltios: objetivo en % / 100 × tensión de alimentación
4. Longitud máxima de ida: L máx = caída permitida / (2 × I × R)

L es la longitud de ida en metros, I la corriente en amperios y R la resistencia del cable en ohmios por metro (el valor de la tabla en Ω/km dividido entre 1000). En corriente continua, vatios divididos entre voltios dan amperios.

Un objetivo habitual es el 3 % para un circuito derivado. NFPA 70 (la NEC), edición 2023, sugiere el 3 % para un circuito derivado y el 5 % para alimentador y derivado juntos, en notas informativas de los artículos 210 y 215. Son solo recomendaciones. Puedes fijar un objetivo más estricto, por ejemplo para electrónica sensible o iluminación LED.

## Resistencia del cobre en los ejemplos

Los valores son para cobre macizo a 20 °C. Se calculan con la fórmula pública del diámetro AWG y la resistividad del cobre recocido. En la [tabla AWG a mm²](awg-to-mm2-chart) se explica cómo se obtienen.

| AWG | mm² | Ω/km |
|---|---|---|
| 12 | 3,31 | 5,21 |
| 10 | 5,26 | 3,28 |
| 8 | 8,37 | 2,06 |
| 6 | 13,3 | 1,30 |
| 4 | 21,2 | 0,815 |

## Ejemplo resuelto: carga de 240 W a 5 m de la batería

Una carga de 12 V consume 240 W. El tendido mide 5 m de ida. Cable de cobre, objetivo del 3 %.

1. Corriente: 240 W / 12 V = 20 A.
2. Caída permitida: 3 % × 12 V = 0,36 V.
3. Longitud de ida y vuelta: 2 × 5 m = 10 m. Multiplicada por la corriente: 10 × 20 = 200 m·A.
4. Se prueba cada sección:

| AWG | Caída (V) | Caída (%) | ¿Dentro del 3 %? |
|---|---|---|---|
| 12 | 1,04 | 8,7 | No |
| 10 | 0,655 | 5,5 | No |
| 8 | 0,412 | 3,4 | No, por poco |
| 6 | 0,259 | 2,2 | Sí |
| 4 | 0,163 | 1,4 | Sí |

5. La sección más pequeña que cumple es 6 AWG (13,3 mm², siguiente sección normalizada 16 mm²). Caída con 6 AWG: 200 × 0,001297 = 0,259 V, es decir, 2,16 %.

Con 8 AWG la caída es del 3,4 % y no cumple el objetivo del 3 %. Comprueba cada sección antes de redondear.

## Longitud máxima de ida a 20 A, 12 V, 3 %

Aquí se usa L máx = 0,36 / (2 × 20 × R).

| AWG | Longitud máx. (m) |
|---|---|
| 10 | 2,7 |
| 8 | 4,4 |
| 6 | 6,9 |
| 4 | 11,0 |

A 24 V la caída permitida en voltios se duplica. La misma carga necesita la mitad de corriente, así que la longitud máxima con el mismo cable es cuatro veces mayor.

## La intensidad admisible sigue contando

La caída de tensión es solo un límite. El cable también tiene que soportar la corriente, y el interruptor automático tiene que proteger el cable. En cargas continuas la NEC exige dimensionar el circuito para el 125 % de la carga (NFPA 70, edición 2023, 210.19(A)(1) y 215.2(A)(1)). Cumplir la caída de tensión no sustituye la comprobación de la intensidad admisible. Vale la mayor de las dos secciones.

## Circuitos de corriente alterna

En corriente alterna la fórmula usa la impedancia en lugar de la resistencia simple:

- Ohmios efectivos por metro: R × cos θ + X × sen θ, donde cos θ es el factor de potencia, R la resistencia y X la reactancia.
- Monofásica: el factor 2 se mantiene.
- Trifásica: el factor 2 pasa a √3 (1,732).

La NEC da R y X en el capítulo 9, tabla 9. La tabla 8 recoge las resistencias en continua. Los valores de las tablas de arriba salen de la fórmula pública a 20 °C, así que difieren un poco de las tablas de la NEC y, en el límite, el resultado puede variar una sección.

## Úsalo en la app

Calculadora de cable (la app está en inglés) hace esta cuenta sin cobertura. Introduce amperios, o vatios y voltios, la longitud y tu objetivo. Comprueba la caída de tensión, la ampacidad, las reglas del interruptor y la clasificación de los terminales, y muestra cuál fijó la sección. Usa la tabla 8 del capítulo 9 de la NEC para CC y la tabla 9 para CA, y cita la tabla y la edición en cada resultado. La app tiene además dos modos inversos: longitud máxima para un cable elegido y carga máxima para un cable y una longitud. Los valores predefinidos de CC cubren 12 V y 24 V, y se ofrecen 18 AWG y 16 AWG para CC. La longitud se elige en metros o en pies.

Los resultados son estimaciones. Verifícalos con la normativa local y la autoridad competente.
