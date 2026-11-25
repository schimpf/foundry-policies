# Der Monarch guía de cosecha y alimentación con fórmulas

> Cuánto grano necesita tu pueblo en Der Monarch, cómo cultivos y suelo fijan la cosecha y cómo la comida cambia la población. Con ejemplos.

- Web: https://apps.schimpf.es/der-monarch/es/der-monarch-feeding-and-harvest-guide/
- App: Der Monarch, https://apps.schimpf.es/der-monarch/es/index.md
El grano que das a tu pueblo y lo que siembras deciden la mayoría de los años en Der Monarch. Esta guía recoge las fórmulas del juego y calcula la situación de partida.

## Cuánto grano necesita la gente

La necesidad es de 7 fanegas por persona. En el juego la fanega aparece como Scheffel (abreviado «Sch.»). Cuentan los siervos, los mercaderes, el clero y la nobleza.

**necesidad = habitantes × 7**

Al empezar tienes 2.140 habitantes, así que la necesidad es 2.140 × 7 = 14.980 fanegas. En el almacén hay 18.000.

La pantalla Volk ernähren (alimentar al pueblo) tiene un deslizador y botones rápidos para el 80 %, la necesidad y el 125 %. El grano que reservas para alimentar no se puede vender.

## Qué hace la comida con la población

Sea proporción = grano repartido / necesidad. El juego calcula el cambio anual así:

- **Nacimientos:** siervos × 3 % × la proporción, con la proporción limitada a 1,2
- **Muertes:** habitantes × 1,5 %
- **Muertos de hambre:** si la proporción es menor que 1, habitantes × (1 − proporción) × 25 %
- **Migración:** (proporción limitada a 1,5 − 1) × habitantes × 8 %, más (30 − presión fiscal) × habitantes × 0,15 %, más el ánimo de la justicia × habitantes

La presión fiscal es (aduanas + impuesto sobre la renta) / 2. El ánimo de la justicia es +0,01 con Milde, 0 con Gerecht, −0,01 con Streng y −0,03 con Grausam. Un resultado positivo de migración son inmigrantes y uno negativo es gente que se marcha.

### Ejemplo: tres niveles de alimentación

Situación de partida: 1.820 siervos, 2.140 habitantes, aduanas 20 %, impuesto sobre la renta 25 %, justicia Gerecht. La presión fiscal es 22,5, así que la parte de los impuestos en la migración es 7,5 × 2.140 × 0,0015 = 24.

| Repartido | Proporción | Nacimientos | Muertes | Muertos de hambre | Migración | Cambio neto |
|---|---|---|---|---|---|---|
| 80 % (11.984) | 0,8 | 44 | 32 | 107 | −10 | **−105** |
| 100 % (14.980) | 1,0 | 55 | 32 | 0 | +24 | **+47** |
| 125 % (18.725) | 1,25 | 66 | 32 | 0 | +67 | **+101** |

Alimentar al 125 % exige 18.725 fanegas, más que las 18.000 que tienes, así que al empezar solo lo alcanzas si compras grano. El deslizador se detiene en el grano que posees. Al cerrar el año, el grano repartido queda limitado a lo que te queda tras las ratas más la cosecha.

Por encima del 120 % ya no hay más nacimientos, pero la migración sigue subiendo hasta el 150 %.

## Qué siembras

Repartes tu tierra entre patatas, grano y avena. El resto queda en barbecho. Cada cultivo se sortea una vez al año entre un rendimiento bajo y uno alto por Morgen (unidad de superficie alemana).

| Cultivo | Rendimiento por Morgen | Riesgo | Desgaste del suelo |
|---|---|---|---|
| Kartoffeln (patatas) | 2,6–3,5 | bajo | 8 |
| Korn (grano) | 1,8–5,2 | alto | 6 |
| Hafer (avena) | 2,5–2,7 | ninguno | 3 |

La fuerza del suelo va del 40 al 100 %. Cada rendimiento se multiplica por suelo / 100. La dificultad inclina el sorteo: Milde da mejores años, Hart da peores y más pérdidas por las ratas.

### Los siervos limitan tus campos

Cada siervo puede trabajar como máximo 6 Morgen. Si quieres sembrar más tierra que siervos × 6, todos los cultivos se reducen en proporción. Con 1.820 siervos puedes trabajar 10.920 Morgen.

### Ejemplo: el plan por defecto

Tierra 10.000 Morgen, plan 40 % patatas, 35 % grano, 15 % avena, 10 % barbecho, suelo 100 %.

1. Sembrado: 4.000 de patatas, 3.500 de grano, 1.500 de avena. En total 9.000 Morgen, por debajo del límite de 10.920.
2. Cosecha mínima: 4.000 × 2,6 + 3.500 × 1,8 + 1.500 × 2,5 = 10.400 + 6.300 + 3.750 = 20.450 fanegas
3. Cosecha máxima: 4.000 × 3,5 + 3.500 × 5,2 + 1.500 × 2,7 = 14.000 + 18.200 + 4.050 = 36.250 fanegas
4. Tu necesidad es de 14.980, así que incluso el peor año alimenta a todos, antes de las ratas.

Las ratas se comen después una parte del grano que tienes, hasta un 5 % en Milde, un 10 % en Normal y un 16 % en Hart.

## Suelo

Cada año el suelo cambia en:

**% de barbecho × 0,6 − Σ(% de cultivo × desgaste / 100)**, redondeado

Con el plan por defecto: desgaste = 0,40 × 8 + 0,35 × 6 + 0,15 × 3 = 5,75. El barbecho aporta 10 × 0,6 = 6. El cambio es +0,25, que se redondea a 0, y el suelo se queda en 100.

Si siembras toda la tierra (0 % de barbecho) solo con patatas, el suelo baja 8 puntos al año. A los 5 años está en 60 y todos los rendimientos son un 40 % más bajos. El suelo nunca baja de 40.

## Consejos

- La avena es el cultivo seguro. El grano rinde entre 1,8 y 5,2 por Morgen.
- Deja algo de barbecho si cultivas a fondo. El barbecho devuelve 0,6 puntos de suelo por cada punto porcentual.
- El grano también se vende. Una buena cosecha se convierte en táleros para construir. Mira los [requisitos de rango](der-monarch-rank-requirements).
- La guerra cuesta cosecha. Cada compañía que envías recorta tu cosecha un 2 %.

## Pruébalo

Der Monarch es un juego de Android para uno a cuatro jugadores en un mismo dispositivo. Todo el texto del juego está en alemán. Abre las pantallas Volk ernähren y Felder bestellen (sembrar los campos) para probar estas cifras.
