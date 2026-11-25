# Calculadora de la media de tensión arterial en casa

> Calcula la media de tus tomas de tensión arterial en casa, con la mínima, la máxima y la categoría AHA. Incluye la fórmula y un ejemplo resuelto.

- Web: https://apps.schimpf.es/health-connect-pdf-reports/es/average-blood-pressure-calculator/
- App: Health Reports: PDF de salud, https://apps.schimpf.es/health-connect-pdf-reports/es/index.md
Un médico suele querer la media de varias tomas hechas en casa. Esta página ofrece una calculadora sencilla para una lista de tomas, y después explica la fórmula y un ejemplo resuelto para que puedas comprobarlo a mano.

## Calculadora

Escribe una toma por línea como sistólica/diastólica, por ejemplo `122/78`. Nada de lo que escribes sale de tu navegador.

An interactive calculator is on the web page: https://apps.schimpf.es/health-connect-pdf-reports/es/average-blood-pressure-calculator/

## La fórmula

La sistólica y la diastólica se promedian por separado.

- Media sistólica = suma de todos los valores sistólicos ÷ número de tomas
- Media diastólica = suma de todos los valores diastólicos ÷ número de tomas

Cada resultado se redondea al número entero más cercano, y el .5 se redondea hacia arriba. La toma mínima y la máxima son las que tienen el valor sistólico más bajo y más alto. Si dos tomas tienen la misma sistólica, decide la diastólica.

Después se coloca la media en una categoría con los límites de la AHA.

| Categoría | Sistólica | | Diastólica |
|---|---|---|---|
| Normal | menos de 120 | y | menos de 80 |
| Elevada (Elevated) | 120–129 | y | menos de 80 |
| Etapa 1 (Stage 1) | 130–139 | o | 80–89 |
| Etapa 2 (Stage 2) | 140 o más | o | 90 o más |
| Por encima de 180/120 (Above 180/120) | más de 180 | y/o | más de 120 |

La AHA es la Asociación Americana del Corazón. Las guías europeas (ESC/ESH) y las sociedades españolas usan otros nombres y otros límites. La app y esta página usan los de la AHA.

Fuente: Whelton PK, et al. *2017 ACC/AHA/AAPA/ABC/ACPM/AGS/APhA/ASH/ASPC/NMA/PCNA Guideline for the Prevention, Detection, Evaluation, and Management of High Blood Pressure in Adults*. Hypertension, 2018; 71(6): e13–e115.

## Ejemplo resuelto

Siete tomas de la mañana a lo largo de una semana:

| Día | Toma |
|---|---|
| Lunes | 128/82 |
| Martes | 122/78 |
| Miércoles | 135/85 |
| Jueves | 126/80 |
| Viernes | 131/84 |
| Sábado | 120/76 |
| Domingo | 124/79 |

### Paso 1: suma los valores sistólicos

128 + 122 + 135 + 126 + 131 + 120 + 124 = 886

### Paso 2: suma los valores diastólicos

82 + 78 + 85 + 80 + 84 + 76 + 79 = 564

### Paso 3: divide entre el número de tomas

- 886 ÷ 7 = 126,57, que se redondea a 127
- 564 ÷ 7 = 80,57, que se redondea a 81

La media es 127/81.

### Paso 4: busca la mínima y la máxima

- Sistólica más baja: 120/76
- Sistólica más alta: 135/85

### Paso 5: coloca la media en una categoría

La sistólica 127 está en la fila 120–129. La diastólica 81 está en la fila 80–89. Los dos números apuntan a filas distintas, así que gana la categoría más alta: Etapa 1.

La misma semana caería en Elevada si la media diastólica hubiera sido 79 o menos. Uno o dos puntos pueden llevar una media al otro lado de un límite, así que conviene mirar la lista completa y la media.

## Categoría de la media y categoría de cada toma

La calculadora promedia primero los números y categoriza después. También puedes categorizar cada toma por separado. En el ejemplo:

- Etapa 1: 128/82, 135/85, 126/80, 131/84 (4 tomas)
- Elevada: 122/78, 120/76, 124/79 (3 tomas)
- Normal, Etapa 2 y Por encima de 180/120: 0 tomas

La categoría de la media y el recuento por categoría pueden diferir. Los dos datos sirven para enseñar al médico.

## Consejos para una media útil

- Toma la tensión durante varios días.
- Usa el mismo brazo, el mismo tensiómetro y una hora parecida.
- Incluye todas las tomas válidas. Si quitas las altas, la media no sirve.
- No mezcles tomas de aparatos distintos sin anotarlo. Los tensiómetros pueden diferir en unos pocos mmHg.

Una calculadora no puede juzgar si un valor es un problema para ti. Lleva la lista y la media a tu médico.

## Sin hacer cuentas con la app

Health Connect PDF Reports para Android hace este trabajo con las tomas guardadas en Health Connect. Su página de resumen muestra la media, la tensión mínima y máxima, la tendencia del pulso en reposo, la duración media del sueño y cuántas tomas caen en cada categoría AHA. Las páginas de detalle listan cada toma con su hora y la app de origen. La media usa el mismo método de arriba: sistólica y diastólica promediadas por separado y redondeadas a números enteros. Las tomas que dos apps guardaron para el mismo suceso se unen antes y cuentan una vez.

También puedes añadir una toma a mano en la app. Se guarda en Health Connect. La app está en inglés y llama a las categorías Normal, Elevated, Stage 1, Stage 2 y Above 180/120. Solo muestra valores registrados y no da diagnósticos ni consejos médicos.

Mira también: [Tabla de categorías de tensión arterial](blood-pressure-categories-chart) y [Cómo crear un PDF de tensión arterial desde Health Connect](health-connect-blood-pressure-pdf).
