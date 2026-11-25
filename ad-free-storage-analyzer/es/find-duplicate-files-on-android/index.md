# Cómo encontrar archivos duplicados en Android

> Encuentra archivos duplicados en el móvil Android: cómo una suma SHA-256 demuestra que son copias exactas y qué copia conservar al borrar.

- Web: https://apps.schimpf.es/ad-free-storage-analyzer/es/find-duplicate-files-on-android/
- App: Analizador de almacenamiento, https://apps.schimpf.es/ad-free-storage-analyzer/es/index.md
Los archivos duplicados llenan el móvil sin que te des cuenta. El mismo vídeo guardado dos veces, una descarga repetida o una foto copiada en dos carpetas. Esta página explica cómo encontrar duplicados exactos, cómo comprobar que son copias reales y cómo borrarlos sin perder nada.

## Qué es un duplicado

Un duplicado exacto tiene el mismo contenido, byte a byte. Puede tener otro nombre, otra carpeta u otra fecha. Dos fotos que solo se parecen no son duplicados exactos, porque sus bytes son distintos.

El nombre no sirve para comparar. Dos archivos llamados `IMG_0042.jpg` pueden ser fotos distintas, y un vídeo guardado como `clip.mp4` y `clip (1).mp4` es el mismo archivo con dos nombres. Lo que cuenta es el contenido.

## Paso a paso: encontrar duplicados a mano

1. Abre un gestor de archivos y entra en la carpeta que sospechas, por ejemplo Descargas.
2. Ordena por tamaño, de mayor a menor.
3. Busca archivos con exactamente el mismo tamaño en bytes. El número exacto aparece en los detalles del archivo.
4. Abre los dos archivos y compáralos.
5. Borra la copia que no necesites.

Esto funciona con unos pocos archivos. Con cientos se hace lento. Además, un mismo tamaño no demuestra que dos archivos sean idénticos, porque archivos distintos pueden pesar lo mismo.

## Cómo una suma de comprobación demuestra que dos archivos coinciden

Una suma de comprobación es una huella corta calculada con cada byte de un archivo. SHA-256 es una función hash estándar (NIST, *FIPS PUB 180-4: Secure Hash Standard*, 2015). Da un resultado de 64 caracteres, como `9f86d081…`.

- Los archivos idénticos dan siempre el mismo SHA-256.
- Si un solo byte cambia, el resultado es totalmente distinto.
- Que dos archivos distintos den el mismo resultado no es un problema en la práctica.

Leer cada byte de un archivo grande lleva tiempo, así que un buen analizador trabaja en dos pasos:

1. **Agrupar por tamaño.** Un archivo con un tamaño que no tiene ningún otro no puede ser un duplicado. Se omite.
2. **Calcular el hash solo de los grupos.** Los archivos del mismo tamaño reciben un SHA-256 sobre el archivo completo. El mismo resultado significa copia exacta.

### Ejemplo con números

Tu móvil tiene estos archivos:

| Archivo | Tamaño |
|---|---|
| `viaje.mp4` | 48.201.330 bytes |
| `viaje (1).mp4` | 48.201.330 bytes |
| `clase.mp4` | 48.201.330 bytes |
| `apuntes.pdf` | 2.310.004 bytes |

1. `apuntes.pdf` tiene un tamaño único, así que se omite.
2. Los tres vídeos tienen el mismo tamaño, así que cada uno recibe un SHA-256.
3. `viaje.mp4` y `viaje (1).mp4` dan el mismo resultado. `clase.mp4` da otro.
4. Resultado: un grupo de duplicados con dos archivos. Al borrar una copia recuperas 48.201.330 bytes, unos 48,2 MB.

## Qué copia conservar

Conserva la copia más reciente. Es la que más probablemente editaste o moviste a propósito, y las copias antiguas suelen ser sobras. Si dos copias tienen la misma fecha, da igual cuál conserves, porque el contenido es el mismo.

Conserva siempre al menos una copia de cada grupo. Si borras todas, el archivo desaparece.

## Encontrar duplicados con Storage Analyzer

Storage Analyzer busca duplicados exactos cuando tocas Scan. La app solo está disponible en inglés, así que los nombres de esta página son los que ves en la app. Sigue los dos pasos de arriba:

- Solo se comprueban los archivos de 1 MB (1.000.000 bytes) o más. Los archivos pequeños ocupan poco.
- Los archivos del mismo tamaño se comparan con SHA-256 sobre el archivo completo. Solo aparecen copias reales.
- Los grupos se ordenan por el espacio que ganarías, de mayor a menor.
- La copia más reciente viene preseleccionada para conservarla. Puedes cambiar la elección de cada archivo.
- Siempre se conserva al menos una copia.
- Un archivo que la app no puede leer queda fuera de los resultados. No cuenta como copia.

Los archivos borrados van a la papelera (Trash) de la app. Puedes deshacer justo después de borrar o restaurarlos desde la papelera durante 7 días. Pasado ese tiempo se eliminan definitivamente. Los archivos se mueven dentro del mismo almacenamiento y no se copian, así que es rápido incluso con vídeos grandes. Al desinstalar la app se vacía su papelera, así que restaura antes lo que quieras conservar.

La app solo encuentra duplicados exactos. No detecta fotos parecidas.

## Lista rápida

- Mismo tamaño y misma suma de comprobación significa mismo archivo.
- Conserva la copia más reciente.
- Revisa el grupo antes de borrar.
- Borra primero a la papelera y vacíala más tarde.
