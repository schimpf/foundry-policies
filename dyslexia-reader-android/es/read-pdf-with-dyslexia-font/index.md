# Leer un PDF con fuente para dislexia en Android

> Un PDF fija la fuente y el diseño. Así conviertes un PDF con texto en texto adaptable en Android, y estos son los límites que se aplican.

- Web: https://apps.schimpf.es/dyslexia-reader-android/es/read-pdf-with-dyslexia-font/
- App: Dyslexia Reader: Leer libros, https://apps.schimpf.es/dyslexia-reader-android/es/index.md
Un PDF fija la fuente, el tamaño y el espaciado de la página. No puedes ensanchar las letras ni cambiar la fuente. Para cambiarlas, hay que extraer el texto del PDF y mostrarlo como un libro normal. Esta página explica cómo funciona y dónde falla.

## Por qué los PDF son difíciles de leer

- El diseño es fijo, así que cambiar el tamaño del texto obliga a hacer zoom y a desplazarse de lado.
- Las líneas suelen ser largas y estar muy juntas.
- La fuente es la que eligió el autor.
- Las columnas y las notas al pie rompen el orden de lectura para un lector de pantalla o una herramienta de lectura en voz alta.

Reajustar el texto (reflow) significa que se recoloca en tu pantalla con tu propia fuente y tu propio espaciado.

## Primera comprobación: ¿el PDF contiene texto?

1. Abre el PDF en cualquier visor.
2. Intenta seleccionar una palabra con una pulsación larga.
3. Si puedes seleccionar y copiar palabras, tiene texto. Se puede reajustar.
4. Si toda la página se selecciona como una sola imagen, es un escaneo. No tiene texto que extraer.

Los PDF escaneados necesitan primero OCR (reconocimiento de texto). Dyslexia Reader Android no hace OCR, así que no admite PDF escaneados sin texto.

## Pasos en Dyslexia Reader Android

La interfaz de la aplicación está en inglés, por eso los nombres aparecen aquí en inglés.

1. Abre la aplicación y ve a la Library (biblioteca).
2. Elige importar un libro y selecciona tu PDF en el dispositivo.
3. Mira la pantalla de importación. Muestra el tamaño del texto y el tiempo de lectura.
4. Abre el libro. Ya se aplican tu fuente y tu espaciado.
5. Abre el panel Appearance (apariencia) para ajustar la fuente, el tamaño del texto y el espaciado.

La importación de PDF necesita la compra única. La importación de TXT y EPUB funciona sin ella.

## Qué se conserva y qué se pierde

| Se conserva | No se conserva |
|---|---|
| El texto, en párrafos | Las imágenes |
| Tu fuente y tu espaciado | El diseño de página |
| La posición de lectura y el progreso | Las columnas y el diseño de la página |
| Lectura en voz alta con frase resaltada | El texto dentro de imágenes escaneadas |

## Límites

La aplicación rechaza los archivos que superan estos límites y te dice el motivo.

- Tamaño de archivo de hasta 100 MB.
- Hasta 3000 páginas.
- Hasta 5 000 000 de caracteres de texto.
- Un PDF protegido con contraseña no se puede abrir. Uno sin contraseña de apertura funciona con normalidad.
- Un archivo dañado se notifica como corrupto.

## Consejos para mejores resultados

- Usa PDF exportados desde un procesador de textos o desde una página web. Conservan el texto limpio.
- Los artículos a dos columnas pueden mezclar las columnas. Si el orden parece incorrecto, busca una versión EPUB o de texto del mismo documento.
- Los encabezados y pies de página de cada hoja pueden repetirse en el texto. Pásalos de largo o lee con la regla activada.
- En documentos largos, usa la lectura en voz alta con frase resaltada para seguir el texto. Usa la voz instalada en tu dispositivo y funciona sin conexión.

## Si la importación falla

- Demasiado grande: el archivo, el número de páginas o el texto superan uno de los límites de arriba. Divide el PDF en partes con una herramienta de PDF e importa cada parte.
- Contraseña: quita la contraseña con una herramienta de PDF y vuelve a importar.
- Escaneado: el PDF no tiene texto. Ejecuta OCR antes en un ordenador o busca una versión en texto en la fuente original.
- Corrupto: descarga el archivo de nuevo, o ábrelo en un visor de PDF y vuelve a guardarlo.

## Revisa el resultado antes de leer

Abre las primeras páginas y fíjate en tres cosas. ¿Los párrafos están en el orden correcto? ¿Hay palabras partidas por saltos de línea raros? ¿Se repite el texto del encabezado? Si el texto se ve limpio, ajusta tu fuente y tu espaciado y empieza a leer. Si no, prueba con otra copia del documento.

## Otras formas de traer texto

- Comparte texto sin formato desde otra aplicación a la biblioteca.
- Importa un archivo TXT.
- Importa un EPUB. Conserva los capítulos y funciona bien con libros.

## Sobre la aplicación

Dyslexia Reader Android es un lector sin conexión para personas con dislexia, con fuentes pensadas para la dislexia, una regla de enfoque de línea, controles de espaciado y lectura en voz alta.

- No hace falta ninguna cuenta.
- Los libros y los ajustes se quedan en tu dispositivo. La aplicación no tiene permiso de internet.
- En Ajustes (Settings) puedes borrar un libro o todos los datos de la aplicación.

Busca Dyslexia Reader: Leer libros en Google Play.
