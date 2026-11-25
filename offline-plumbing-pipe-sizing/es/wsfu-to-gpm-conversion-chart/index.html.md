# Conversión de WSFU a GPM con la curva de Hunter

> Convierte unidades de aparato (WSFU) a GPM y l/min con la curva de Hunter. Valores para cisterna y fluxómetro, con un ejemplo resuelto.

- Web: https://apps.schimpf.es/offline-plumbing-pipe-sizing/es/wsfu-to-gpm-conversion-chart/
- App: Dimensionar tuberías IPC y UPC, https://apps.schimpf.es/offline-plumbing-pipe-sizing/es/index.md
Las unidades de aparato de suministro de agua (WSFU, water supply fixture units) indican cuánta carga pone un aparato sobre una tubería de suministro. Para dimensionar la tubería necesitas el caudal en galones por minuto (GPM). La curva de Hunter une los dos datos. Esta página muestra una tabla de conversión, explica las dos curvas y resuelve un ejemplo a mano.

Equivalencia: 1 GPM = 3,785 l/min. En España el caudal se da en l/s o l/min, por eso aparecen las dos unidades.

## Qué es la curva de Hunter

No todos los aparatos funcionan a la vez. Roy B. Hunter usó la probabilidad para estimar el caudal punta que un grupo de aparatos consume de verdad. Su trabajo, *Methods of Estimating Loads in Plumbing Systems* (National Bureau of Standards, Building Materials and Structures Report BMS 65, 1940), es de dominio público y sigue siendo la base de las tablas de demanda de los códigos de fontanería de EE. UU.

Hay dos curvas:

- Cisterna, para sistemas en los que los inodoros llevan cisterna. Da un caudal punta menor.
- Fluxómetro (válvula de descarga), para sistemas en los que los inodoros llevan fluxómetro. Da un caudal punta mayor, porque un fluxómetro consume mucha agua en poco tiempo.

Elige la curva según el tipo de inodoro. Un trabajo con fluxómetros usa la curva de fluxómetro en todo el tramo.

## Tabla de WSFU a GPM

Puntos seleccionados de las curvas. Los valores intermedios se obtienen por interpolación lineal. Los datos entre paréntesis son l/min.

| WSFU totales | Cisterna, GPM (l/min) | Fluxómetro, GPM (l/min) |
|---|---|---|
| 5 | 9,4 (35,6) | 15,0 (56,8) |
| 10 | 14,6 (55,3) | 27,0 (102) |
| 20 | 19,6 (74,2) | 35,0 (132) |
| 30 | 23,3 (88,2) | 42,0 (159) |
| 40 | 26,3 (99,6) | 46,0 (174) |
| 50 | 29,1 (110) | 50,0 (189) |
| 100 | 43,5 (165) | 67,5 (256) |
| 200 | 65,0 (246) | 90,0 (341) |
| 300 | 85,0 (322) | 108,0 (409) |
| 500 | 124,0 (469) | 143,0 (541) |
| 1000 | 208,0 (787) | 208,0 (787) |

Notas sobre los rangos:

- La curva de cisterna va de 1 a 5000 WSFU. Con 1 WSFU son 3,0 GPM y con 2 WSFU, 5,0 GPM.
- La curva de fluxómetro va de 5 a 5000 WSFU.
- Las dos curvas coinciden a partir de 1000 WSFU. Los sistemas grandes tienen tantos aparatos que el tipo de inodoro ya no cambia el caudal punta.

## Cómo convertir

1. Suma las WSFU de todos los aparatos que atiende la tubería, con los valores del código vigente.
2. Elige la curva de cisterna o la de fluxómetro.
3. Busca los dos puntos de la tabla a cada lado de tu total.
4. Interpola entre ellos.

La interpolación es:

**GPM = GPM₁ + (WSFU − WSFU₁) / (WSFU₂ − WSFU₁) × (GPM₂ − GPM₁)**

## Ejemplo resuelto

Un grupo de baños en un sistema con cisterna suma 22 WSFU.

1. Los puntos de la tabla a cada lado son 20 WSFU (19,6 GPM) y 25 WSFU (21,5 GPM).
2. La posición entre ellos es (22 − 20) / (25 − 20) = 0,4.
3. GPM = 19,6 + 0,4 × (21,5 − 19,6) = 19,6 + 0,76 = 20,36, que se redondea a 20,4 GPM (77,2 l/min, 1,29 l/s).

Las mismas 22 WSFU en un sistema con fluxómetro:

1. Puntos: 20 WSFU (35,0 GPM) y 25 WSFU (38,0 GPM).
2. GPM = 35,0 + 0,4 × (38,0 − 35,0) = 36,2 GPM (137 l/min, 2,28 l/s).

El sistema con fluxómetro necesita casi 16 GPM (unos 60 l/min) más para las mismas unidades de aparato.

## Qué hacer con el caudal

El caudal por sí solo no da el tamaño de la tubería. Después se compara la velocidad de cada tamaño con un límite y se mira la pérdida de carga. Las fórmulas están en la página de Hazen-Williams de este sitio.

Por ejemplo, 20,4 GPM en cobre tipo L (diámetro interior de 1,025 pulgadas para 1", es decir 26,0 mm) dan una velocidad de 0,4085 × 20,4 / 1,025² = 7,9 fps (2,4 m/s). Queda justo dentro del límite de 8 fps (2,44 m/s) para agua fría, así que 1" sirve. Con 36,2 GPM la misma tubería circularía a 14,1 fps (4,3 m/s) y necesitarías 1-1/2" (6,5 fps, 2,0 m/s).

## Límites del método

- La curva de Hunter da una estimación punta para mezclas habituales de aparatos. Las cargas continuas, como el riego o el agua de proceso, se suman aparte.
- Los aparatos modernos de bajo consumo suelen gastar menos de lo que predice la curva. Los códigos siguen usando la curva, así que sigue el código vigente.
- Tu código vigente decide qué valores de aparatos y qué edición se aplican. El IPC (edición 2024) trata la demanda en el Apéndice E, sección E103.3. El UPC (edición 2024) la trata en el Apéndice A, sección A 103.0.
- Las tablas impresas de los códigos pueden diferir ligeramente de los valores de la curva calculados así.
- En España el caudal de cálculo se obtiene según el CTE DB HS 4, con el caudal instantáneo de cada aparato y un coeficiente de simultaneidad, y no con WSFU. Esta tabla sirve para los códigos de EE. UU. y no sustituye ese método.

## Convierte y dimensiona en la app

La app para Android Offline Plumbing Pipe Sizing hace esta conversión por ti. Introduce las WSFU totales, elige una vez cisterna o fluxómetro y la app convierte a GPM con la curva de Hunter. Después muestra el tamaño de tubería recomendado, la velocidad y la pérdida de carga en psi por 100 ft de cada tamaño, de 1/2" a 4". Funciona sin conexión y muestra la sección del IPC o del UPC de la edición que elijas. La app está en inglés y calcula solo en unidades de EE. UU.

## Fuentes

- Hunter, R. B., *Methods of Estimating Loads in Plumbing Systems*, National Bureau of Standards, Building Materials and Structures Report BMS 65, 1940.
- International Plumbing Code (ICC), 2024 edition, Appendix E.
- Uniform Plumbing Code (IAPMO), 2024 edition, Appendix A.
- Código Técnico de la Edificación, Documento Básico HS 4, Suministro de agua.
