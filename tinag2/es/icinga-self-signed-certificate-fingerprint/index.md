# Huella SHA-256 de un certificado autofirmado de Icinga

> Cómo obtener con openssl la huella SHA-256 (fingerprint) del certificado autofirmado de un servidor Icinga 2 o Thruk y usarla en la app Android.

- Web: https://apps.schimpf.es/tinag2/es/icinga-self-signed-certificate-fingerprint/
- App: Tinag2: Alertas Icinga/Nagios, https://apps.schimpf.es/tinag2/es/index.md
Muchos servidores Icinga 2 usan un certificado autofirmado. El móvil no confía en él y las conexiones fallan. La solución segura es fijar el certificado: le das al cliente la huella SHA-256 exacta que debe aceptar y dejas activada la comprobación de certificados. Esta página explica cómo obtener esa huella y qué comprobar antes de fiarte de ella.

## Qué es una huella

La huella de un certificado es un hash del archivo del certificado en su forma binaria (DER). SHA-256 produce 32 bytes, que se muestran como 64 caracteres hexadecimales, a menudo en pares separados por dos puntos:

`3A:9F:...:C1` (32 pares)

Dos certificados distintos no comparten huella. Si se sustituye el certificado del servidor, la huella cambia.

## Obtener la huella con openssl

Necesitas un ordenador que llegue al servidor y tenga OpenSSL instalado.

1. Elige el nombre de host y el puerto. La API de Icinga 2 escucha por defecto en el puerto 5665 (documentación de Icinga 2, capítulo "Icinga 2 API"). Thruk y la mayoría de las interfaces web usan el puerto 443.
2. Ejecuta este comando con tu propio host y puerto:

```
openssl s_client -connect icinga.example.com:5665 -servername icinga.example.com </dev/null 2>/dev/null | openssl x509 -noout -fingerprint -sha256
```

3. La salida tiene este aspecto:

```
sha256 Fingerprint=3A:9F:12:...:C1
```

4. Copia la parte que va después del signo igual.

El comando toma el primer certificado que presenta el servidor, que es el certificado propio del servidor (el certificado hoja). Es el que debes fijar.

## Compruébalo antes de fiarte

Leer la huella por la red significa fiarse de quien haya respondido. En una red no fiable, alguien podría responder en lugar de tu servidor. Para estar seguro:

- Ejecuta el comando desde una red de confianza, idealmente la LAN del servidor o el propio servidor.
- O compara con el archivo del certificado en el servidor. En Icinga 2, el certificado de la API está en el directorio de datos de Icinga 2 (normalmente `/var/lib/icinga2/certs/`). Ejecuta `openssl x509 -in <archivo> -noout -fingerprint -sha256` sobre él y compara los dos valores.

## Usar la huella en Tinag2

Tinag2 es un cliente Android para Icinga 2 y para Nagios/Naemon a través de Thruk. Cada servidor que añades puede tener una huella fijada opcional.

1. Abre **Instances** y pulsa **Add instance**, o edita uno existente.
2. Introduce el nombre, el tipo, la URL, el usuario y la contraseña.
3. Pega la huella en el campo "Trusted certificate SHA-256 (optional)".
4. Guarda y actualiza.

La aplicación compara la huella con el SHA-256 del certificado que presenta el servidor. Ignora los dos puntos y las mayúsculas o minúsculas, así que puedes pegar la salida de openssl tal cual, sin el prefijo `sha256 Fingerprint=`.

## Qué hace y qué no hace fijar la huella

- El certificado hoja del servidor se acepta si su huella coincide con la que fijaste. Cualquier otro certificado debe superar la comprobación normal del sistema.
- Con una huella fijada, la aplicación no exige que el nombre de host coincida con el del certificado. La huella identifica al servidor. Esto ayuda cuando te conectas por dirección IP o con un nombre interno que el certificado no incluye.
- La huella fijada vale solo para ese servidor. Los demás servidores de la aplicación mantienen su propia configuración.
- También se permite HTTP sin cifrar en redes locales. El diálogo de la instancia te avisa, porque las contraseñas enviadas por HTTP se pueden leer en la red. Una conexión HTTPS con huella fijada es mejor.

## Cuando la conexión falla después de haber funcionado

La causa más común es un certificado nuevo. Los certificados de Icinga 2 y de Thruk caducan, y un certificado renovado o regenerado tiene una huella nueva. Ejecuta de nuevo el comando openssl y actualiza la huella fijada.

Otras causas:

- Acceso rechazado (HTTP 401 o 403): el usuario o la contraseña son incorrectos, o el usuario de la API no tiene permisos.
- API no encontrada (HTTP 404): la URL base es incorrecta. Para Icinga 2 usa la dirección de la API con el puerto, como `https://icinga.example.com:5665`. Para Thruk usa la raíz de Thruk, como `https://mon.example.com/thruk`.
- No se alcanza el host: el móvil no está en una red que llegue al servidor, por ejemplo porque la VPN está apagada.

Tinag2 muestra los problemas de tu servidor Icinga 2 o Thruk, te deja reconocerlos, volver a comprobarlos y programar un mantenimiento, y te avisa de los problemas nuevos o que han empeorado. Tus contraseñas se cifran con el Android Keystore, y la aplicación solo habla con los servidores que introduces.
