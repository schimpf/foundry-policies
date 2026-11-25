# Tabla de tuberías de cobre y PEX por caudal (GPM)

> Caudal máximo en GPM y l/min de tuberías de cobre tipo L y PEX, de 1/2 a 4 pulgadas, a 5 y 8 fps, con diámetros interiores y un ejemplo resuelto.

- Web: https://apps.schimpf.es/offline-plumbing-pipe-sizing/es/copper-and-pex-pipe-size-chart-gpm/
- App: Dimensionar tuberías IPC y UPC, https://apps.schimpf.es/offline-plumbing-pipe-sizing/es/index.md
Una tubería de cobre tipo L de 3/4" transporta hasta 12,07 GPM (45,7 l/min) a 8 fps y hasta 7,54 GPM (28,5 l/min) a 5 fps. El máximo depende del límite de velocidad que aceptes y del diámetro interior real de la tubería. Esta página reúne una tabla del caudal máximo por tamaño para cobre tipo L y PEX, explica cómo salen las cifras y dimensiona una línea a partir de un caudal dado.

Equivalencias: 1 GPM = 3,785 l/min, 1 fps = 0,3048 m/s, 1 pulgada = 25,4 mm.

## Por qué la velocidad fija el tamaño

Para dimensionar el suministro de agua se suele elegir la tubería más pequeña que mantiene la velocidad por debajo de un límite. El agua rápida hace ruido y desgasta la tubería, sobre todo en las líneas de agua caliente. Hay dos límites habituales:

- 8 fps (2,44 m/s) para agua fría.
- 5 fps (1,52 m/s) para agua caliente en cobre.

El IPC no indica un límite de velocidad para estos materiales. Los valores proceden de recomendaciones de fabricantes y de la Copper Development Association (*Copper Tube Handbook*). El UPC (ediciones 2024 y 2021, Apéndice A, sección A 105.1) indica 8 fps para agua fría. La autoridad local decide qué se aplica, así que confírmalo antes de fiarte de un límite.

## La fórmula detrás de la tabla

Despeja el caudal en la ecuación de la velocidad para obtener lo que transporta una tubería a una velocidad dada:

**GPM = velocidad en fps × d² / 0,4085**

Aquí d es el diámetro interior en pulgadas. A 8 fps, GPM = 19,58 × d². A 5 fps, GPM = 12,24 × d².

## Diámetros interiores

Los diámetros interiores proceden de ASTM B88 (cobre tipo L) y ASTM F876 (PEX, SDR 9). El tamaño nominal es solo una etiqueta. Los valores corresponden a tubería estadounidense. El tubo de cobre europeo según UNE-EN 1057 y los tubos PEX con medidas en mm tienen otros diámetros interiores.

## Caudal máximo, cobre tipo L

Los datos entre paréntesis son l/min. Los DN son equivalencias aproximadas.

| Tamaño nominal | Diám. interior en pulgadas (mm) | GPM máx. (l/min) a 8 fps (frío) | GPM máx. (l/min) a 5 fps (caliente) |
|---|---|---|---|
| 1/2" (DN 15) | 0,545 (13,8) | 5,82 (22,0) | 3,64 (13,8) |
| 3/4" (DN 20) | 0,785 (19,9) | 12,07 (45,7) | 7,54 (28,5) |
| 1" (DN 25) | 1,025 (26,0) | 20,58 (77,9) | 12,86 (48,7) |
| 1-1/4" (DN 32) | 1,265 (32,1) | 31,34 (119) | 19,59 (74,2) |
| 1-1/2" (DN 40) | 1,505 (38,2) | 44,36 (168) | 27,72 (105) |
| 2" (DN 50) | 1,985 (50,4) | 77,17 (292) | 48,23 (183) |
| 2-1/2" (DN 65) | 2,465 (62,6) | 119,0 (450) | 74,37 (282) |
| 3" (DN 80) | 2,945 (74,8) | 169,9 (643) | 106,2 (402) |
| 4" (DN 100) | 3,905 (99,2) | 298,6 (1130) | 186,6 (706) |

## Caudal máximo, PEX (SDR 9)

En las recomendaciones usadas aquí, el PEX no tiene un límite de 5 fps para agua caliente. Una columna a 8 fps sirve para los dos casos.

| Tamaño nominal | Diám. interior en pulgadas (mm) | GPM máx. (l/min) a 8 fps |
|---|---|---|
| 1/2" (DN 15) | 0,475 (12,1) | 4,42 (16,7) |
| 3/4" (DN 20) | 0,671 (17,0) | 8,82 (33,4) |
| 1" (DN 25) | 0,862 (21,9) | 14,55 (55,1) |
| 1-1/4" (DN 32) | 1,054 (26,8) | 21,76 (82,4) |
| 1-1/2" (DN 40) | 1,244 (31,6) | 30,31 (115) |
| 2" (DN 50) | 1,629 (41,4) | 51,97 (197) |
| 2-1/2" (DN 65) | 2,011 (51,1) | 79,20 (300) |
| 3" (DN 80) | 2,400 (61,0) | 112,8 (427) |
| 4" (DN 100) | 3,162 (80,3) | 195,8 (741) |

Compara las dos tablas. Con el mismo tamaño nominal, el PEX transporta menos porque sus paredes son más gruesas y su diámetro interior es menor. Una línea de PEX de 1" transporta unos 14,5 GPM (55 l/min) a 8 fps, y una de cobre L de 1" transporta unos 20,6 GPM (78 l/min).

## Cómo usar la tabla

1. Busca tu caudal de diseño en GPM (1 l/min = 0,2642 GPM). Si tienes unidades de aparato, conviértelas con la curva de Hunter (consulta la página de WSFU a GPM de este sitio).
2. Elige el material y el límite de velocidad.
3. Baja por la columna hasta el primer tamaño cuyo caudal máximo sea igual o mayor que tu caudal.

## Ejemplo resuelto

Una línea de agua caliente debe transportar 14,6 GPM (55,3 l/min, 0,92 l/s) en cobre tipo L, con el límite de 5 fps para agua caliente.

1. 3/4" admite como máximo 7,54 GPM, así que se queda corta.
2. 1" admite como máximo 12,86 GPM, y también se queda corta.
3. 1-1/4" admite como máximo 19,59 GPM. Es el primer tamaño que sirve.

Comprueba la velocidad: 0,4085 × 14,6 / 1,265² = 3,7 fps (1,14 m/s). El mismo caudal en una línea de agua fría a 8 fps cabe en 1" (5,7 fps, 1,73 m/s).

## Comprueba también la pérdida de carga

La velocidad es solo una parte de la comprobación, porque los tramos largos pierden presión. La pérdida de carga de Hazen-Williams del ejemplo de agua fría anterior (14,6 GPM, cobre L de 1", C = 130) es de unos 6,99 psi por 100 ft (1,58 kPa/m). En un tramo de 60 ft (18,3 m) son unos 4,2 psi (29 kPa). La página de Hazen-Williams de este sitio muestra el cálculo completo.

## Límites de esta tabla

- Los valores son calculados y pueden diferir ligeramente de las tablas impresas.
- Los tamaños mínimos del código siguen vigentes. Por ejemplo, el IPC 2024 fija 3/4" como mínimo para una acometida (sección 603.1) y el UPC 2024 fija 3/4" para el suministro del edificio (sección 610.8). Un resultado de 1/2" en la tabla no anula ese mínimo.
- Los accesorios, los contadores, los desniveles y la presión de red no forman parte de esta tabla.
- En España el dimensionado se rige por el CTE DB HS 4, que fija para tuberías metálicas una velocidad de 0,50 a 2,00 m/s (hasta 6,6 fps). Esta tabla usa tubería estadounidense y los límites de 8 y 5 fps, y no sustituye ese cálculo.

## Usa la app en lugar de la tabla

La app para Android Offline Plumbing Pipe Sizing construye esta tabla para tu caudal exacto. Introduce GPM o WSFU, elige IPC o UPC, la edición 2024 o 2021 y un material. Marca el tamaño más pequeño dentro del límite de velocidad y muestra la velocidad y los psi por 100 ft de cada tamaño, de 1/2" a 4". Puedes cambiar el límite de velocidad entre 1 y 20 fps y volver al valor por defecto. Funciona sin conexión. El cobre L y el PEX están disponibles desde el primer arranque. El cobre K y M, el CPVC, el PEX-AL-PEX, el PE-RT y los trabajos guardados forman parte de la compra única Pro. La app está en inglés y calcula solo en unidades de EE. UU.

## Fuentes

- ASTM B88, Standard Specification for Seamless Copper Water Tube (inside diameters, Type L).
- ASTM F876, Standard Specification for Crosslinked Polyethylene (PEX) Tubing (SDR 9 inside diameters).
- Copper Development Association, *Copper Tube Handbook* (velocity guidance for copper).
- International Plumbing Code (ICC), 2024 edition, section 603.1.
- Uniform Plumbing Code (IAPMO), 2024 edition, sections 610.8 and Appendix A, A 105.1.
- Código Técnico de la Edificación, Documento Básico HS 4, Suministro de agua.
