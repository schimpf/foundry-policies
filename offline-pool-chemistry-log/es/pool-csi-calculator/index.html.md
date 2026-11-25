# Calculadora CSI de piscina: índice de saturación

> Calcula el índice de saturación de calcita (CSI) del agua de tu piscina con la fórmula, un ejemplo resuelto y qué cambiar cuando se desvía.

- Web: https://apps.schimpf.es/offline-pool-chemistry-log/es/pool-csi-calculator/
- App: Pool Chem Log: Pruebas de agua, https://apps.schimpf.es/offline-pool-chemistry-log/es/index.md
El índice de saturación de calcita (CSI) indica si el agua de tu piscina tiende a disolver el revoco y el metal o a dejar cal. Un CSI cercano a cero significa agua equilibrada. Esta página te ofrece una calculadora, la fórmula y un ejemplo resuelto.

## Calculadora CSI

An interactive calculator is on the web page: https://apps.schimpf.es/offline-pool-chemistry-log/es/pool-csi-calculator/

## Cómo leer el resultado

- **Por debajo de -0,3:** corrosiva. El agua puede atacar el revoco, dañar las juntas y deteriorar las piezas metálicas.
- **De -0,3 a +0,3:** equilibrada. Este es el margen que Pool Chem Log usa como objetivo.
- **Por encima de +0,3:** incrustante. El calcio puede depositarse en azulejos, superficies y en la célula de sal o el calentador.

El margen de -0,3 a +0,3 es un objetivo práctico. Las piscinas de revoco son las que más ganan si se mantienen dentro de él.

## Qué entra en el CSI

El CSI usa estos resultados de prueba:

- pH
- Alcalinidad total (TA), en ppm
- Dureza cálcica (CH), en ppm (si tu prueba da grados franceses, 1 °f equivale a 10 ppm)
- Ácido cianúrico (CYA), en ppm
- Boratos, en ppm (opcional)
- Sal, en ppm
- Temperatura del agua, en °C

El agua caliente incrusta con más facilidad, así que la temperatura importa. La sal tiene un efecto pequeño a través de la fuerza iónica. Si no conoces tu nivel de sal, la calculadora supone 1.000 ppm, un valor típico del agua de llenado más los subproductos del cloro. Si dejas CYA o boratos en blanco, cuentan como 0. 1 ppm equivale a 1 mg/l.

## La fórmula

La fórmula es la que usan Trouble Free Pool (TFP) y Pool Math, atribuida al químico conocido como "chem geek".

CSI = pH - 6,9395 + log10(CH) + log10(alcalinidad de carbonatos) - 2,56 × sqrt(I) / (1 + 1,65 × sqrt(I)) - 1412,5 / T

Donde:

- **Alcalinidad de carbonatos** = TA - 0,38772 × CYA / (1 + 10^(6,83 - pH)) - 4,63 × boratos / (1 + 10^(9,11 - pH)). El CYA y los boratos cuentan como TA en un kit de análisis, pero no ayudan al equilibrio de los carbonatos, por eso se restan.
- **I (fuerza iónica)** = (1,5 × CH + TA) / 50045 + sal / 58440.
- **T** es la temperatura del agua en kelvin: grados Celsius + 273,15.

Si CH es 0 o la alcalinidad de carbonatos sale en 0 o menos, no se puede calcular el CSI.

## Ejemplo resuelto

Una piscina de revoco da estos resultados:

- pH 7,5
- TA 70 ppm
- CH 350 ppm
- CYA 40 ppm
- Boratos 0
- Sal 1.000 ppm (supuesta)
- Agua a 27 °C, es decir, 300,15 K

Paso a paso:

1. Alcalinidad de carbonatos: 10^(6,83 - 7,5) = 0,2138, así que la parte del CYA = 0,38772 × 40 / 1,2138 = 12,78. Alcalinidad de carbonatos = 70 - 12,78 = 57,22.
2. Fuerza iónica: (1,5 × 350 + 70) / 50045 + 1000 / 58440 = 0,01189 + 0,01711 = 0,02900. Su raíz cuadrada es 0,1703.
3. Término iónico: 2,56 × 0,1703 / (1 + 1,65 × 0,1703) = 0,4360 / 1,2810 = 0,3403.
4. Término de temperatura: 1412,5 / 300,15 = 4,7060.
5. Logaritmos: log10(350) = 2,5441 y log10(57,22) = 1,7576.
6. Suma: 7,5 - 6,9395 + 2,5441 + 1,7576 - 0,3403 - 4,7060 = -0,18.

El CSI es de aproximadamente -0,18. Está dentro del margen equilibrado, algo hacia el lado blando.

## Qué cambiar cuando el CSI se desvía

Si el CSI es demasiado bajo (corrosivo), sube uno de estos valores:

- **Dureza cálcica:** la palanca más fuerte en piscinas de revoco. El cloruro de calcio la sube, pero despacio, así que añádelo por etapas.
- **pH:** subir el pH 0,1 sube el CSI en cerca de 0,1.
- **Alcalinidad total:** el bicarbonato de sodio la sube.

Si el CSI es demasiado alto (incrustante), baja el pH con ácido o baja la TA. Bajar el calcio exige cambiar agua, porque ningún producto lo elimina.

Los objetivos de calcio en Pool Chem Log dependen de la superficie:

| Superficie | Rango de CH (ppm) |
|---|---|
| Revoco o grava | 250 a 650 |
| Vinilo o fibra de vidrio | 50 a 350 |
| Acrílico | 150 a 250 (rango habitual) |

Los rangos de revoco, grava, vinilo y fibra de vidrio siguen las pautas de TFP. El rango del acrílico es un rango habitual del sector.

## Boratos y sal

Los boratos son opcionales. Algunos propietarios mantienen de 30 a 50 ppm como amortiguador del pH. Si los usas, inclúyelos en el cálculo, porque los boratos suben la lectura de TA sin mejorar el equilibrio. Las piscinas de agua salada deben introducir su nivel real de sal.

## Límites

El CSI es un modelo y depende de pruebas precisas, sobre todo de TA, CH y pH. Un error pequeño en una prueba puede mover el CSI 0,1 o más. Repite la prueba antes de cambiar algo importante, nunca mezcles productos químicos, usa protección y sigue la etiqueta del producto.

## Sigue el CSI con el tiempo

Pool Chem Log es una app de Android que funciona sin conexión. Calcula el CSI con cada prueba que introduces, con boratos y sal incluidos, y usa la temperatura de la última prueba. También muestra tus objetivos según el tipo de superficie, calcula dosis de calcio, alcalinidad y pH, y guarda un historial de todas tus pruebas. La fórmula de la app es la misma que la de esta página.
