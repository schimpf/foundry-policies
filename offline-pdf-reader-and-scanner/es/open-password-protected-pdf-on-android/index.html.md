# Abrir un PDF con contraseña en Android

> Por qué un PDF pide contraseña, qué versiones de Android lo abren, qué hacer si falla y la diferencia entre las dos contraseñas de un PDF.

- Web: https://apps.schimpf.es/offline-pdf-reader-and-scanner/es/open-password-protected-pdf-on-android/
- App: Lector y escáner de PDF, https://apps.schimpf.es/offline-pdf-reader-and-scanner/es/index.md
Tocas un PDF y te pide una contraseña, o no se abre. Que puedas abrirlo depende de la contraseña y de tu versión de Android. Esta página trata ambas cosas.

## Dos tipos de contraseña en un PDF

La especificación PDF (ISO 32000-1:2008, sección 7.6, e ISO 32000-2:2020 para PDF 2.0) define dos contraseñas:

| Contraseña | Qué hace |
| --- | --- |
| **Contraseña de usuario (apertura)** | Hace falta para abrir el archivo y leerlo. |
| **Contraseña de propietario (permisos)** | Fija límites, como no imprimir o no copiar. El archivo se abre sin ella. |

Un lector solo te pide contraseña cuando el archivo tiene una contraseña de usuario. La eligió quien envió el archivo. Nadie puede leerla dentro del archivo, y la app no puede recuperar una contraseña perdida.

## Qué versiones de Android pueden abrirlos

En Offline PDF reader and scanner, la respuesta depende del motor PDF del sistema:

| Versión de Android | PDF con contraseña |
| --- | --- |
| Android 15 (API 35) y posteriores | Se abre tras introducir la contraseña |
| Android 14 (API 34) y anteriores | No es compatible. La app muestra un mensaje. |

En versiones anteriores, la app muestra «Los PDF con contraseña requieren Android 15» y explica que el dispositivo no puede abrirlos. No adivina la contraseña ni busca atajos.

## Cómo abrir uno en Android 15 o posterior

1. Abre el PDF desde tus archivos, un adjunto de correo o una app de la nube. Usa **Abrir con** y elige la app, o selecciona el archivo desde dentro de la app.
2. Un cuadro de diálogo muestra **Se necesita contraseña**.
3. Escribe la contraseña y toca **Abrir**.
4. Si es incorrecta, la app muestra **Contraseña incorrecta**. Inténtalo de nuevo.

Las contraseñas distinguen mayúsculas de minúsculas. Comprueba si hay un espacio al final cuando la copias de un mensaje.

## Si no tienes la contraseña

- Pregunta a quien te envió el archivo. Bancos, empresas y administraciones suelen usar una regla, como la fecha de nacimiento, el DNI o el número de cliente. Su correo o su carta normalmente indica cuál.
- No busques programas para descifrar contraseñas de archivos que no son tuyos. Muchos no son seguros, y abrir el archivo protegido de otra persona puede ser ilegal.
- Si el archivo es tuyo y perdiste la contraseña, la fuente original (por ejemplo, la banca online de tu banco) suele poder darte una copia nueva.

## Si falla en una versión anterior de Android

Tienes tres opciones:

1. Actualiza el móvil a Android 15 si el fabricante lo ofrece.
2. Abre el archivo en un ordenador, donde la mayoría de los lectores PDF aceptan una contraseña.
3. Pide a quien te lo envió una copia sin contraseña de usuario, si el contenido no es confidencial.

## Qué más funciona con el archivo abierto

- Desplazamiento vertical continuo y retomar la lectura en la última página.
- El índice, si el archivo lo tiene.
- Búsqueda de texto, si el PDF tiene capa de texto. Si es un escaneo, el reconocimiento de texto (Pro) le añade una.
- Páginas nocturnas, que invierten los colores de la página para leer a oscuras.

La app guarda dónde lo dejaste para que puedas volver más tarde. Los archivos recientes solo recuerdan dónde está un PDF. La app no sube ni cambia el original, y puedes borrar la lista de recientes en Ajustes.

## Privacidad de los archivos protegidos

La apertura ocurre en el dispositivo. La app no tiene permiso de internet, así que ni el archivo ni la contraseña que escribes se envían a ningún sitio.

## Preguntas

### ¿Por qué el mismo PDF se abre en mi navegador pero no aquí?

Algunos navegadores y lectores de escritorio traen su propio motor PDF. En Android, la app usa el motor del sistema, que admite contraseñas desde Android 15.

### ¿La contraseña de propietario me impide leer?

No. Un archivo con solo contraseña de propietario se abre sin pedirla. Los límites afectan a acciones como imprimir.

### ¿La app quita la contraseña?

No. Solo abre el archivo para que puedas leerlo.

## Pruébalo

Offline PDF reader and scanner está en Google Play. Abre un PDF protegido e introduce la contraseña.
