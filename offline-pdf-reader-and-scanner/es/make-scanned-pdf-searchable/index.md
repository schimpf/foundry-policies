# Cómo hacer buscable un PDF escaneado en Android (OCR)

> Por qué no se puede buscar en un PDF escaneado, cómo el OCR añade una capa de texto y cómo hacerlo buscable en tu móvil sin subir el archivo.

- Web: https://apps.schimpf.es/offline-pdf-reader-and-scanner/es/make-scanned-pdf-searchable/
- App: Lector y escáner de PDF, https://apps.schimpf.es/offline-pdf-reader-and-scanner/es/index.md
Escaneas un contrato, lo abres, buscas una palabra y aparece «Sin coincidencias». La página muestra palabras, pero el archivo solo contiene una imagen de ellas. Esta página explica por qué ocurre, cómo comprobarlo y cómo solucionarlo en Android sin subir el archivo a ningún sitio.

## Por qué un PDF escaneado no tiene texto buscable

Una página PDF puede contener dos tipos de contenido:

- **Objetos de texto.** Caracteres reales con fuente y posición. Buscar, copiar y resaltar funcionan sobre ellos.
- **Imágenes.** Una foto de la página. Tus ojos leen las palabras, pero el archivo no contiene ningún carácter.

Un escaneo con la cámara produce solo una imagen. Un PDF exportado desde Word o desde una página web suele tener texto real. Por eso la búsqueda falla en los escaneos y funciona en los documentos hechos en el ordenador.

## Cómo comprobar si tu PDF tiene capa de texto

1. Abre el PDF en un lector.
2. Busca una palabra que veas en la página.
3. Intenta seleccionar una línea con una pulsación larga.

Si la búsqueda no encuentra nada y no puedes seleccionar texto, la página es solo una imagen.

## Qué hace el OCR

OCR significa reconocimiento óptico de caracteres. El software mira la imagen, encuentra líneas de texto y averigua qué caracteres son. Después escribe esos caracteres en el PDF como una capa invisible sobre la imagen.

- La página se ve exactamente igual.
- Buscar, copiar y resaltar ya funcionan en la página.
- La imagen original se queda en el archivo.

La precisión depende del escaneo. Las páginas nítidas, planas y bien iluminadas con texto impreso dan los resultados más exactos. Las fotos borrosas, las sombras, la letra manuscrita y las fuentes poco comunes producen más errores.

## Hacer buscable un escaneo con Offline PDF reader and scanner

La app ejecuta el reconocimiento de texto en tu móvil con el modelo latino de Google ML Kit incluido en la app. No se sube nada, y la app no tiene permiso de internet. El reconocimiento de texto es una función Pro (pago único).

### Opción 1: automáticamente tras cada escaneo

1. Abre **Ajustes** y comprueba que **Hacer buscables los escaneos** está activado. Al desbloquear Pro, viene activado por defecto.
2. Toca **Escanear documento** en la pantalla de inicio.
3. Escanea las páginas y toca **Guardar escaneo**.
4. El reconocimiento de texto empieza tras guardar. El progreso aparece en la fila del escaneo en la biblioteca.

El resultado sustituye al escaneo, así que tienes un solo archivo por escaneo.

### Opción 2: un PDF que ya tienes

1. Abre en el lector el PDF que solo contiene imágenes.
2. Busca una palabra. La app te avisa de que no hay capa de texto y te pregunta si quieres hacerlo buscable.
3. Confirma. La app inicia el reconocimiento de texto.

En un PDF importado, la app guarda el resultado como una copia en la biblioteca con el nombre «(buscable)». El archivo original no cambia.

### Opción 3: después de añadir páginas

Si añades páginas a un escaneo guardado en el editor de páginas, las páginas nuevas también pasan por el reconocimiento de texto. Al guardar se sustituye el escaneo.

## Qué ocurre durante el reconocimiento

- Cada página se renderiza con 2480 píxeles de ancho. En una página A4 son unos 300 ppp, una resolución habitual para OCR.
- El modelo del alfabeto latino lee cada página y devuelve líneas de texto con sus posiciones.
- La app escribe todas las líneas en el PDF como texto invisible y después sustituye el archivo una sola vez.
- Se ejecuta como trabajo normal en segundo plano. Puedes salir de la app mientras termina.
- Si tarda más de 30 minutos o falla, el escaneo se marca como fallido. El archivo queda como estaba.

Los documentos largos tardan más, porque cada página se procesa una por una.

## Límites que conviene conocer

- **Solo alfabeto latino.** Funcionan el español, el inglés, el alemán y otros idiomas que usan letras latinas. El cirílico, el griego, el árabe, el chino, el japonés y el coreano no son compatibles.
- **Solo Pro.** Leer, escanear sin más y buscar en PDF que ya tienen texto no requieren Pro.
- **Servicios de Google Play.** Escanear y Pro los necesitan. Leer PDF funciona sin ellos.
- **Revisa las cifras importantes.** El OCR puede leer un 5 como un 6. Compara importes, fechas y números de identificación con la página.

## Tras el reconocimiento: buscar y resaltar

Cuando una página tiene capa de texto, puedes:

1. Tocar el icono de búsqueda en el lector y escribir una palabra.
2. Usar los botones de siguiente y anterior para saltar entre coincidencias.
3. Mantener pulsado y arrastrar sobre el texto para resaltarlo. Los resaltados son anotaciones PDF estándar, así que otros lectores también los muestran. La app los guarda como copia en tu biblioteca y nunca cambia el original.

## Preguntas

### ¿El OCR hace el archivo más grande?

Un poco. La capa de texto es pequeña comparada con las imágenes de las páginas.

### ¿Puedo buscar antes del OCR?

No. Sin capa de texto no hay nada que buscar. Ejecuta primero el reconocimiento.

### ¿Se envía mi escaneo a un servidor?

No. El reconocimiento se ejecuta en el móvil, y la app no tiene permiso de internet.

## Pruébalo

Offline PDF reader and scanner está en Google Play. Escanea una página, espera a que termine el reconocimiento y busca una palabra en ella.
