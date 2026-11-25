# Fórmula del tiempo estándar con ejemplo resuelto

> Cómo calcular el tiempo normal y el tiempo estándar a partir de lecturas del cronómetro, valoración y suplemento, con ejemplo resuelto y calculadora.

- Web: https://apps.schimpf.es/time-study-stopwatch/es/standard-time-formula-example/
- App: Estudio de Tiempos Cronómetro, https://apps.schimpf.es/time-study-stopwatch/es/index.md
El tiempo estándar es el que necesita un operario formado para hacer una tarea a ritmo normal, más el tiempo de descanso y de demoras inevitables. Es la cifra que hay detrás de los estándares de mano de obra, el equilibrado de líneas y la planificación de capacidad. Esta página da la fórmula, un ejemplo resuelto con números reales y una calculadora que puedes usar ahora mismo.

## La fórmula

El tiempo estándar se calcula en dos pasos.

1. Tiempo normal = tiempo observado × valoración ÷ 100
2. Tiempo estándar = tiempo normal × (1 + suplemento ÷ 100)

Donde:

- El tiempo observado es lo que marca el cronómetro para un elemento.
- La valoración es tu juicio sobre el ritmo del operario. 100 % significa ritmo normal. Más de 100 % es más rápido que lo normal, menos de 100 % es más lento.
- El suplemento es el tiempo extra para necesidades personales, fatiga y demoras (PF&D), como porcentaje del tiempo normal.

El método sigue los manuales clásicos de medición del trabajo, por ejemplo Niebel y Freivalds, *Methods, Standards, and Work Design* (McGraw-Hill, 12.ª edición, 2009), y la Oficina Internacional del Trabajo, *Introducción al estudio del trabajo* (4.ª edición, 1992).

### Reglas que usan la app y esta página

- El tiempo normal se calcula por elemento. Cada observación se multiplica por su valoración y después se hace la media.
- Los tiempos normales de todos los elementos se suman para obtener el tiempo normal del ciclo.
- El suplemento es un recargo sobre el tiempo normal. Un suplemento del 15 % multiplica el tiempo normal por 1,15.
- El suplemento se acepta de 0 a 100 %.
- La valoración se acepta de 50 a 200 %.

Algunas fuentes definen el suplemento como una parte de toda la jornada. En esa versión, tiempo estándar = tiempo normal ÷ (1 − suplemento ÷ 100), que da resultados distintos. La fórmula de esta página es la del recargo.

## Ejemplo resuelto

Se cronometra a un operario de empaquetado en una tarea con dos elementos, durante tres ciclos. Cada observación tiene una valoración.

| Elemento | Ciclo | Observado (s) | Valoración (%) | Observado × valoración (s) |
|---|---|---|---|---|
| 1. Coger el artículo | 1 | 20 | 110 | 22,00 |
| 1. Coger el artículo | 2 | 22 | 100 | 22,00 |
| 1. Coger el artículo | 3 | 18 | 120 | 21,60 |
| 2. Embalar y cerrar | 1 | 40 | 90 | 36,00 |
| 2. Embalar y cerrar | 2 | 44 | 100 | 44,00 |
| 2. Embalar y cerrar | 3 | 42 | 95 | 39,90 |

### Paso 1: tiempo normal por elemento

- Elemento 1: (22,00 + 22,00 + 21,60) ÷ 3 = 21,87 s
- Elemento 2: (36,00 + 44,00 + 39,90) ÷ 3 = 39,97 s

### Paso 2: tiempo normal del ciclo

- 21,87 + 39,97 = 61,83 s

Compáralo con la media observada sin valorar: 20 s + 42 s = 62 s. La valoración cambió poco el resultado porque los valores altos y bajos se compensan en parte. Con un operario que sea siempre rápido o siempre lento, la diferencia es mayor.

### Paso 3: aplicar el suplemento

Con un suplemento del 15 %:

- 61,83 × 1,15 = 71,11 s

El tiempo estándar de un ciclo de embalaje es de unos 71,1 segundos. Con ese estándar, un operario hace unos 50 ciclos por hora (3600 ÷ 71,11 = 50,6).

## Calculadora

An interactive calculator is on the web page: https://apps.schimpf.es/time-study-stopwatch/es/standard-time-formula-example/

## Errores frecuentes

- Valorar al trabajador en lugar del ritmo. Valora la velocidad y el esfuerzo del trabajo que ves. Valora cada observación mientras la miras.
- Saltarse la valoración. Sin ella obtienes la media de cómo trabajó este operario ese día, que todavía no es un estándar.
- Mezclar métodos de suplemento. Comprueba si tu empresa define el suplemento sobre el tiempo normal o sobre toda la jornada antes de comparar cifras.
- Muy pocos ciclos. Tres ciclos bastan para una demostración. Para un estándar real, usa más ciclos y mira la dispersión. Una desviación estándar grande indica que el método o los elementos aún no son estables.
- Cronometrar ciclos incompletos. Cuenta solo los ciclos en los que se cronometró cada elemento, para que el total del ciclo no quede por debajo.

## Hazlo en la app

Time Study Stopwatch aplica esta misma fórmula en la pantalla de resultados. Defines los elementos de trabajo una vez, tocas el botón grande de vuelta cada vez que termina un elemento y ajustas una valoración por observación. Introduce el suplemento en la pantalla de configuración del estudio y la app muestra el tiempo normal por elemento, el tiempo normal del ciclo y el tiempo estándar.

Media, mínimo, máximo y desviación estándar por elemento vienen incluidos en la app. La valoración (50 a 200 %), el suplemento y el tiempo estándar forman parte de Time Study Pro, una compra única en Google Play. Tus datos se quedan en el dispositivo, y la exportación CSV te permite llevar las cifras a una hoja de cálculo.
