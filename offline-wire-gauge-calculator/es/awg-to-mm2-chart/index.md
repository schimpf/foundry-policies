# Tabla AWG a mm²: sección, equivalente métrico y resistencia

> Convierte AWG a mm² con una tabla de área, sección métrica siguiente y resistencia del cobre, más la fórmula y un ejemplo resuelto.

- Web: https://apps.schimpf.es/offline-wire-gauge-calculator/es/awg-to-mm2-chart/
- App: Calculadora de cable: NEC, https://apps.schimpf.es/offline-wire-gauge-calculator/es/index.md
Un AWG es una posición en una escala. Cuanto mayor es el número, más fino es el cable. Esta página ofrece una tabla de conversión de 18 AWG a 250 kcmil, la fórmula que hay detrás y una calculadora pequeña para cualquier tamaño.

## Tabla AWG a mm² (cobre)

La columna "Sección métrica siguiente" indica la menor sección métrica normalizada que es igual o mayor que la del cable AWG. Solo empareja tamaños y no dimensiona un circuito.

| AWG | Área (mm²) | Sección métrica siguiente (mm²) | Ω/km | Ω por 1000 ft |
|---|---|---|---|---|
| 18 | 0,823 | 1 | 20,9 | 6,39 |
| 16 | 1,31 | 1,5 | 13,2 | 4,01 |
| 14 | 2,08 | 2,5 | 8,29 | 2,53 |
| 12 | 3,31 | 4 | 5,21 | 1,59 |
| 10 | 5,26 | 6 | 3,28 | 0,999 |
| 8 | 8,37 | 10 | 2,06 | 0,628 |
| 6 | 13,3 | 16 | 1,30 | 0,395 |
| 4 | 21,2 | 25 | 0,815 | 0,248 |
| 2 | 33,6 | 35 | 0,513 | 0,156 |
| 1/0 | 53,5 | 70 | 0,322 | 0,0983 |
| 2/0 | 67,4 | 70 | 0,256 | 0,0779 |
| 3/0 | 85,0 | 95 | 0,203 | 0,0618 |
| 4/0 | 107 | 120 | 0,161 | 0,0490 |
| 250 kcmil | 127 | 150 | 0,136 | 0,0415 |

La resistencia es la de un conductor macizo de cobre a 20 °C. El aluminio tiene unas 1,64 veces la resistencia del cobre con el mismo tamaño, porque su conductividad es el 61 % de la del cobre.

## Cómo funciona el AWG

Cada paso hacia un número AWG menor hace el cable más grueso. Cada 6 pasos el diámetro se reduce a la mitad, más o menos, y cada 3 pasos el área se duplica, más o menos. De ahí salen unas comprobaciones rápidas:

- 10 AWG tiene unos 5,3 mm². Tres pasos más grueso (7 AWG) tendría unos 10,6 mm², el doble de área.
- De 12 AWG a 6 AWG el área se cuadruplica más o menos (de 3,31 a 13,3 mm²).
- Los tamaños por encima de 4/0 se dan en kcmil. Un kcmil son 0,5067 mm².

## La fórmula

El diámetro AWG se define con una progresión geométrica entre 36 AWG y 0000 (4/0) AWG. La usa la norma ASTM B258, *Standard Specification for Standard Nominal Diameters and Cross-Sectional Areas of AWG Sizes of Solid Round Wires Used as Electrical Conductors*.

1. Diámetro en mm: d = 0,127 × 92^((36 − n) / 39), donde n es el número de calibre. Usa n = 0 para 1/0, −1 para 2/0, −2 para 3/0 y −3 para 4/0.
2. Área en mm²: A = π / 4 × d².
3. Para tamaños en kcmil: A = kcmil × 0,5067.
4. Resistencia en Ω/km: ρ / A × 1000, con ρ = 1/58 Ω·mm²/m para cobre recocido (100 % IACS, International Annealed Copper Standard) y ρ = (1/58) / 0,61 para aluminio (61 % IACS).
5. Ω por 1000 ft = Ω/km × 0,3048.

### Ejemplo resuelto: 10 AWG de cobre

1. n = 10, así que d = 0,127 × 92^(26 / 39) = 0,127 × 92^0,6667 = 0,127 × 20,38 = 2,588 mm.
2. A = π / 4 × 2,588² = 5,26 mm².
3. Resistencia = (1 / 58) / 5,26 × 1000 = 3,28 Ω/km.
4. En pies: 3,28 × 0,3048 = 0,999 Ω por 1000 ft.
5. La menor sección métrica igual o mayor que 5,26 mm² es 6 mm².

## Secciones métricas

La columna "Sección métrica siguiente" usa las secciones nominales de IEC 60228, *Conductors of insulated cables*. Son 0,5, 0,75, 1, 1,5, 2,5, 4, 6, 10, 16, 25, 35, 50, 70, 95, 120, 150, 185, 240, 300, 400, 500, 630, 800 y 1000 mm². Los tamaños AWG y métricos rara vez coinciden, así que al sustituir un cable se suele redondear a la siguiente sección métrica. Comprueba por separado la intensidad admisible del cable métrico. El área sola no la determina, porque el aislamiento, el método de instalación y la temperatura ambiente la modifican.

## Convierte cualquier tamaño

An interactive calculator is on the web page: https://apps.schimpf.es/offline-wire-gauge-calculator/es/awg-to-mm2-chart/

## Límites de esta tabla

- La tabla muestra un conductor macizo. Los conductores de varios hilos tienen la misma sección nominal, pero un diámetro exterior algo mayor y una resistencia algo más alta.
- La resistencia es a 20 °C. La del cobre sube un 0,39 % por °C, así que un cable a 75 °C tiene un 22 % más de resistencia, más o menos.
- Los cálculos de caída de tensión de la NEC usan los valores de resistencia de NFPA 70, capítulo 9, tabla 8 (edición 2023), que son para otra temperatura y para conductores sin recubrir. Difieren un poco de las cifras de arriba. Esta página no reproduce tablas de la NEC.

## Consúltalo en la app

Calculadora de cable lleva esta tabla integrada en Reference, para cobre y aluminio, en mm² y en Ω por km y por 1000 ft. Funciona sin cobertura. La app está en inglés. La misma app también calcula la sección del cable según las reglas de la NEC de ampacidad, caída de tensión e interruptor automático. Cada resultado muestra qué límite fijó la sección y de qué tabla y edición de la NEC procede. Los resultados son estimaciones. Verifícalos con la normativa local y la autoridad competente.
