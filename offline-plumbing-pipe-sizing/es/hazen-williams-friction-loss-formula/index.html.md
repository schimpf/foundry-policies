# Fórmula de Hazen-Williams para la pérdida de carga

> Fórmula de Hazen-Williams para la pérdida de carga en tuberías de agua, con valores C del cobre y el PEX, conversión a kPa/m y un ejemplo.

- Web: https://apps.schimpf.es/offline-plumbing-pipe-sizing/es/hazen-williams-friction-loss-formula/
- App: Dimensionar tuberías IPC y UPC, https://apps.schimpf.es/offline-plumbing-pipe-sizing/es/index.md
Hazen-Williams es la forma habitual de estimar la pérdida de carga en tuberías de suministro de agua. Es sencilla, trabaja en unidades de EE. UU. y es suficientemente precisa para dimensionar líneas de agua fría y caliente. Esta página da la fórmula, los valores C que se usan para el cobre y el plástico, y un ejemplo resuelto que puedes seguir con una calculadora.

Equivalencias: 1 GPM = 3,785 l/min, 1 fps = 0,3048 m/s, 1 ft = 0,3048 m, 1 pulgada = 25,4 mm, 1 psi = 6,895 kPa, 1 psi por 100 ft = 0,2262 kPa/m.

## La fórmula

Para agua en una tubería llena, la pérdida de carga en psi por cada 100 pies de tubería es:

**psi por 100 ft = 100 × 4,52 × Q^1,852 / (C^1,852 × d^4,8704)**

Donde:

- Q es el caudal en galones por minuto (GPM).
- C es el coeficiente de rugosidad de Hazen-Williams. Un C mayor indica una tubería más lisa.
- d es el diámetro interior real de la tubería en pulgadas. El tamaño nominal no entra en la fórmula.

La fórmula procede del trabajo de Williams y Hazen (*Hydraulic Tables*, 1905). La forma de arriba es la versión habitual en unidades de EE. UU. que aparece en las referencias de fontanería y protección contra incendios.

Para obtener la pérdida en un tramo, escala por la longitud:

**pérdida en psi = psi por 100 ft × longitud en ft / 100**

Esto vale solo para tubería recta. Los accesorios, las válvulas y los contadores añaden pérdidas que esta fórmula no incluye.

## Velocidad

La velocidad importa tanto como la fricción. El agua rápida causa ruido y erosión, y por eso casi todo dimensionado parte de un límite de velocidad.

**velocidad en fps = 0,4085 × Q / d²**

Q va en GPM y d es el diámetro interior en pulgadas.

## Valores C que se usan

Valores de diseño, inferiores a los mejores casos de tubería nueva:

| Material | C |
|---|---|
| Cobre (tipos K, L, M) | 130 |
| PEX, PE-RT, CPVC, PEX-AL-PEX | 150 |

## Usa el diámetro interior

El tamaño nominal es solo un nombre. El tubo de cobre se designa por su diámetro nominal, y el diámetro interior real cambia con el tipo de pared. Estos son los diámetros interiores que se usan en esta página, según ASTM B88 (cobre tipo L) y ASTM F876 (PEX, SDR 9). Corresponden a tubería estadounidense. El tubo de cobre europeo según UNE-EN 1057 tiene otros diámetros interiores.

| Tamaño nominal | Cobre L, diám. interior en pulgadas (mm) | PEX SDR 9, diám. interior en pulgadas (mm) |
|---|---|---|
| 1/2" (DN 15) | 0,545 (13,8) | 0,475 (12,1) |
| 3/4" (DN 20) | 0,785 (19,9) | 0,671 (17,0) |
| 1" (DN 25) | 1,025 (26,0) | 0,862 (21,9) |
| 1-1/4" (DN 32) | 1,265 (32,1) | 1,054 (26,8) |
| 1-1/2" (DN 40) | 1,505 (38,2) | 1,244 (31,6) |
| 2" (DN 50) | 1,985 (50,4) | 1,629 (41,4) |

Los DN son equivalencias aproximadas. Como la fricción depende de d elevado a 4,87, un pequeño cambio del diámetro interior tiene un gran efecto. Una línea de PEX suele ser un tamaño mayor que la de cobre para el mismo caudal.

## Ejemplo resuelto

Un ramal atiende 10 unidades de aparato (WSFU, water supply fixture units) con cisternas. Según la curva de Hunter, 10 WSFU son 14,6 GPM (55,3 l/min). La tubería es de cobre tipo L (C = 130) y el límite de velocidad para agua fría es de 8 fps (2,44 m/s). El tramo mide 60 ft (18,3 m).

Paso 1, comprobar cada tamaño. Calcula la velocidad con 0,4085 × 14,6 / d², que es 5,964 / d²:

| Tamaño | Diám. interior en pulgadas | Velocidad en fps (m/s) | Pérdida en psi/100 ft (kPa/m) | ¿Dentro de 8 fps? |
|---|---|---|---|---|
| 1/2" | 0,545 | 20,1 (6,1) | 152 (34,4) | No |
| 3/4" | 0,785 | 9,68 (2,95) | 25,6 (5,79) | No |
| 1" | 1,025 | 5,68 (1,73) | 6,99 (1,58) | Sí |

Paso 2, elegir el tamaño más pequeño dentro del límite. Es 1".

Paso 3, calcular a mano la pérdida de 1".

1. 14,6^1,852 = 143,3
2. 130^1,852 = 8223
3. 1,025^4,8704 = 1,128
4. psi por 100 ft = 100 × 4,52 × 143,3 / (8223 × 1,128) = 64 785 / 9274 = 6,99

Paso 4, escalar a 60 ft. 6,99 × 60 / 100 = 4,19 psi de pérdida en el tramo recto (28,9 kPa, casi 0,29 bar).

El mismo caudal en cobre de 3/4" perdería 25,6 psi por 100 ft y circularía a casi 10 fps (cerca de 3 m/s). Por eso la comprobación de la velocidad va primero.

## Pruébalo

An interactive calculator is on the web page: https://apps.schimpf.es/offline-plumbing-pipe-sizing/es/hazen-williams-friction-loss-formula/

La calculadora usa las fórmulas y los diámetros interiores de arriba y trabaja en GPM, pulgadas, pies y psi. Los resultados son valores calculados y pueden diferir ligeramente de las tablas impresas.

## Qué no cubre esta página

- Accesorios y válvulas. Suma su pérdida aparte.
- Desniveles y presión de red.
- Agua que no sea agua potable normal a temperaturas habituales.

Consulta el código de fontanería vigente y a la autoridad local para las reglas de dimensionado y los tamaños mínimos. Por ejemplo, el IPC (edición 2024) trata el dimensionado de tuberías de agua en la sección 604.3 y el Apéndice E, y el UPC (edición 2024) en la sección 610.1 y el Apéndice A. En España el cálculo de la instalación se rige por el CTE DB HS 4. Hazen-Williams con tubería estadounidense no lo sustituye.

## Calcula en obra

La app para Android Offline Plumbing Pipe Sizing hace este cálculo para todos los tamaños de 1/2" a 4" a la vez. Introduce WSFU o GPM, elige un material y muestra el tamaño recomendado, la velocidad y los psi por 100 ft en una tabla. Si indicas la longitud de un tramo, añade la pérdida total de la tubería recta. Funciona sin conexión y cita la sección del IPC o del UPC de la edición que elijas (2024 o 2021). El cobre L y el PEX están listos desde el primer arranque. La app está en inglés y calcula solo en unidades de EE. UU.

## Fuentes

- Williams, G. S. and Hazen, A., *Hydraulic Tables*, 1905.
- ASTM B88, Standard Specification for Seamless Copper Water Tube (inside diameters, Type L).
- ASTM F876, Standard Specification for Crosslinked Polyethylene (PEX) Tubing (SDR 9 inside diameters).
- International Plumbing Code (ICC), 2024 edition, section 604.3 and Appendix E.
- Uniform Plumbing Code (IAPMO), 2024 edition, section 610.1 and Appendix A.
