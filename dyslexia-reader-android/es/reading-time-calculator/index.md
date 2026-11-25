# Calculadora de tiempo de lectura de un libro

> Calcula cuánto tarda en leerse un libro a partir de sus palabras o caracteres. Fórmula, ejemplos resueltos y una calculadora para probar.

- Web: https://apps.schimpf.es/dyslexia-reader-android/es/reading-time-calculator/
- App: Dyslexia Reader: Leer libros, https://apps.schimpf.es/dyslexia-reader-android/es/index.md
Con una sola división obtienes una buena estimación del tiempo de lectura. Esta página muestra la fórmula, tres ejemplos resueltos y una calculadora que puedes usar aquí mismo.

## La respuesta rápida

- Supón unas 200 palabras por minuto.
- Una palabra cuenta como seis caracteres: cinco letras y un espacio.
- Eso da 1200 caracteres por minuto.
- Divide los caracteres que faltan entre 1200 y redondea hacia arriba a minutos enteros.

Las personas con dislexia suelen leer a menos de 200 palabras por minuto, y la velocidad cambia según el texto. Toma el resultado como un número para planificar. Si lees a 100 palabras por minuto, duplícalo.

An interactive calculator is on the web page: https://apps.schimpf.es/dyslexia-reader-android/es/reading-time-calculator/

## La fórmula

minutos restantes = techo( (caracteres totales - caracteres ya leídos) / 1200 )

- Caracteres totales cuenta letras, cifras, signos de puntuación y espacios.
- Caracteres ya leídos es el punto donde te quedaste.
- Techo redondea hacia arriba. Con 1 solo carácter pendiente el resultado es 1 minuto.
- Si has terminado el libro, el resultado es 0.

Si solo conoces el número de palabras, multiplícalo por 6 para obtener los caracteres.

caracteres = palabras × 6

Es un promedio. Los libros con muchas palabras cortas salen algo altos, y los de palabras largas algo bajos. En un libro entero el error suele ser pequeño.

## Cómo averiguar el número de palabras

- Un archivo TXT: ábrelo en un procesador de textos y lee el recuento en la barra de estado.
- Un documento de un procesador de textos: usa su herramienta de recuento de palabras.
- Un libro publicado: la página de la editorial suele indicarlo. Si no, estímalo por páginas. Una página de libro de bolsillo tiene unas 250 a 300 palabras.
- En Dyslexia Reader Android no necesitas el recuento. La pantalla de importación muestra el tamaño del texto y el tiempo de lectura antes de añadir el libro.

## Porcentaje leído

El progreso es el número de caracteres leídos dividido entre el total, por 100, redondeado hacia abajo.

porcentaje = suelo( caracteres leídos × 100 / caracteres totales )

Al redondear hacia abajo, solo ves 100 % cuando de verdad has llegado al final.

## Ejemplos resueltos

### Una novela de 90 000 palabras

1. Caracteres: 90 000 × 6 = 540 000.
2. Minutos: 540 000 / 1200 = 450.
3. 450 minutos son 7 horas 30 minutos.

### Un cuento, leído en parte

Tienes un texto de 54 000 caracteres y te quedaste en el carácter 20 000.

1. Caracteres restantes: 54 000 - 20 000 = 34 000.
2. Minutos: 34 000 / 1200 = 28,33. Redondeado hacia arriba, 29 minutos.
3. Progreso: 20 000 × 100 / 54 000 = 37,03. Redondeado hacia abajo, 37 %.

### Casi terminado

Te quedan 1000 caracteres.

1. 1000 / 1200 = 0,83.
2. Redondeado hacia arriba: 1 minuto.

## Tabla rápida

Cada fila usa la regla de 200 palabras por minuto.

| Palabras | Caracteres | Tiempo de lectura |
|---|---|---|
| 5000 | 30 000 | 25 min |
| 20 000 | 120 000 | 1 h 40 min |
| 50 000 | 300 000 | 4 h 10 min |
| 90 000 | 540 000 | 7 h 30 min |
| 120 000 | 720 000 | 10 h |

## Ajústalo a tu propia velocidad

Para usar tu propio ritmo, divide las palabras entre tus palabras por minuto en lugar de entre 200.

1. Lee durante un minuto una página de la que conozcas el número de palabras.
2. Cuenta las palabras que has leído. Ese es tu ritmo.
3. Divide las palabras del libro entre ese número.

Ejemplo: un libro de 60 000 palabras a 120 palabras por minuto son 60 000 / 120 = 500 minutos, es decir, 8 horas 20 minutos.

## Dónde lo hace la aplicación por ti

Dyslexia Reader Android calcula este número para cada libro de tu biblioteca. Usa la misma regla de 1200 caracteres por minuto y el mismo redondeo. Ves el progreso y el tiempo restante en cada libro y en el lector. Un widget para la pantalla de inicio muestra lo mismo para el libro que estás leyendo y te lleva de vuelta a donde lo dejaste.

- Importa archivos TXT, EPUB o PDF desde tu dispositivo.
- Todo se queda en tu dispositivo. La aplicación no tiene permiso de internet.
- Incluye un libro de muestra corto para que veas los números antes de añadir los tuyos.

Busca Dyslexia Reader: Leer libros en Google Play.
