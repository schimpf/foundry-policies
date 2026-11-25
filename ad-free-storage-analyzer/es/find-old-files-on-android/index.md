# Cómo encontrar archivos antiguos sin usar en Android

> Encuentra archivos sin cambios desde hace más de 90 días: descargas, capturas, archivos de WhatsApp e instaladores APK. Con reglas y un ejemplo.

- Web: https://apps.schimpf.es/ad-free-storage-analyzer/es/find-old-files-on-android/
- App: Analizador de almacenamiento, https://apps.schimpf.es/ad-free-storage-analyzer/es/index.md
Los archivos antiguos se acumulan en unos pocos sitios previsibles. Descargas que abriste una vez, capturas de pantalla que ya no necesitas, archivos de los chats e instaladores de apps que ya están instaladas. Esta página explica dónde mirar, qué puede significar "antiguo" y cómo limpiar con seguridad.

## Qué significa "antiguo"

Un archivo es antiguo cuando no ha cambiado durante un tiempo fijo. Android guarda una fecha de última modificación para cada archivo. Storage Analyzer considera antiguo un archivo cuando esa fecha queda a más de 90 días en el pasado.

La regla en números: 90 días × 24 horas × 60 minutos × 60 segundos × 1000 milisegundos = 7.776.000.000 ms. Un archivo es antiguo si ahora menos su última modificación es mayor que esa cifra.

### Ejemplo con números

Hoy es 1 de noviembre. Revisa tres archivos:

| Archivo | Última modificación | Hace (días) | ¿Antiguo? |
|---|---|---|---|
| `factura.pdf` | 15 de julio | 109 | Sí |
| `setup.apk` | 10 de septiembre | 52 | No |
| `meme.jpg` | 3 de agosto | 90 | No, exactamente 90 no es más de 90 |

"Última modificación" no es "último acceso". Un archivo que abres a menudo sigue siendo antiguo si nunca lo cambias.

## Dónde se esconden los archivos antiguos

### Descargas

Los navegadores y las apps guardan aquí por defecto. Es la primera carpeta que debes revisar.

### Capturas de pantalla

Las capturas se hacen para un momento concreto y casi nunca se vuelven a usar. Suelen estar en una carpeta llamada Screenshots.

### Archivos de WhatsApp

Las fotos, los vídeos y las notas de voz de los chats se guardan en las carpetas de WhatsApp. En un año pueden ocupar mucho.

### Instaladores APK

Un APK es el archivo de instalación de una app. Cuando la app ya está instalada, el archivo normalmente no hace falta.

## Paso a paso: limpiar a mano

1. Abre un gestor de archivos y entra en Descargas (la carpeta se llama Download).
2. Ordena por fecha, del más antiguo al más reciente.
3. Revisa los archivos de más de 90 días. Borra los que no necesites.
4. Repite con la carpeta Screenshots, las carpetas de WhatsApp y cualquier carpeta con archivos APK.
5. Antes de borrar un documento que quizá necesites otra vez, cópialo a un lugar seguro.

## Encontrar archivos antiguos con Storage Analyzer

Cuando tocas Scan, la app agrupa los archivos antiguos por ti. Solo está disponible en inglés, así que los nombres de los grupos son los que ves en la app:

- **Downloads:** archivos antiguos en la carpeta principal Download o Downloads.
- **Screenshots:** archivos antiguos en cualquier carpeta llamada Screenshots.
- **WhatsApp media:** archivos antiguos en las carpetas de WhatsApp, incluido WhatsApp Business.
- **APK installers:** instaladores antiguos (APK, APKS, XAPK y APKM), salvo que estén en carpetas de Downloads, Screenshots o WhatsApp. En ese caso van a ese grupo.
- **Other old files:** todo lo demás que es antiguo.

"Other old files" deja fuera tus propias carpetas de fotos, vídeos y música: DCIM, Pictures, Movies, Music, Recordings, Podcasts y Audiobooks. Una foto antigua de vacaciones no es basura. Si quieres revisar esos archivos, usa la lista de archivos grandes.

La pantalla de inicio muestra un tamaño recuperable. Suma los archivos antiguos, los instaladores APK y todas las copias duplicadas salvo la más reciente. Los archivos grandes no cuentan, porque un archivo grande no es basura por sí solo.

## Borrar sin riesgo

- Los archivos borrados van a la papelera (Trash) de la app. Usa deshacer al momento o restaura desde la papelera dentro de 7 días.
- Pasados 7 días, los archivos se eliminan definitivamente. La comprobación se hace al abrir la app y una vez al día.
- Los archivos se mueven y no se copian, así que borrar es rápido.
- Las carpetas nunca se borran. Solo los archivos.
- Al desinstalar la app también se vacía su papelera, así que restaura antes lo que quieras conservar.

## Los análisis son manuales

La app solo analiza cuando tocas Scan. Nunca analiza en segundo plano. En modo completo usa el acceso a todos los archivos para revisar cada carpeta del almacenamiento interno y de la tarjeta SD. En modo limitado solo mira las fotos, los vídeos y la música que Android comparte con las apps, así que la lista de archivos antiguos es más corta.

## Lista rápida

- Antiguo significa más de 90 días desde la última modificación.
- Revisa primero Descargas, capturas, archivos de WhatsApp y archivos APK.
- Deja las fotos y la música personales fuera de la basura.
- Borra primero a la papelera y vacíala más tarde.
