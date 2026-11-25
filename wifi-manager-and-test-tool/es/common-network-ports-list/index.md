# Lista de puertos de red comunes y qué significan

> Lista de puertos TCP comunes en redes domésticas, para qué sirve cada servicio y cómo ver qué puertos tiene abiertos un dispositivo de tu red.

- Web: https://apps.schimpf.es/wifi-manager-and-test-tool/es/common-network-ports-list/
- App: Escáner WiFi y herramientas, https://apps.schimpf.es/wifi-manager-and-test-tool/es/index.md
Un puerto es un número que indica a un dispositivo para qué servicio es una conexión de red. Cuando escaneas un dispositivo, un puerto abierto significa que hay un servicio escuchando ahí. Esta página lista los puertos que aparecen a menudo en redes domésticas y de oficinas pequeñas, y explica cómo leer un escaneo.

Los nombres y números de puerto proceden del registro IANA Service Name and Transport Protocol Port Number Registry. Algunos puertos de la lista, como el 5000 y el 9100, se usan más por costumbre que por registro.

## Puertos comunes

| Puerto | Servicio | Qué es |
|---|---|---|
| 21 | FTP | Transferencia de archivos. Sin cifrar. |
| 22 | SSH | Acceso remoto cifrado y copia de archivos. |
| 23 | Telnet | Acceso remoto antiguo. Sin cifrar. |
| 25 | SMTP | Envío de correo entre servidores. |
| 53 | DNS | Resolución de nombres. Los routers suelen responder aquí. |
| 80 | HTTP | Páginas web, incluidas muchas páginas de administración de routers y cámaras. |
| 110 | POP3 | Descarga de correo. Sin cifrar. |
| 139 | NetBIOS | Nombres y archivos compartidos de Windows, antiguo. |
| 143 | IMAP | Descarga de correo. Sin cifrar. |
| 443 | HTTPS | Páginas web cifradas. |
| 445 | SMB | Archivos compartidos de Windows y Samba. |
| 554 | RTSP | Vídeo de cámaras IP. |
| 631 | IPP | Impresión en red. |
| 993 | IMAPS | IMAP sobre TLS. |
| 995 | POP3S | POP3 sobre TLS. |
| 1883 | MQTT | Mensajes entre dispositivos del hogar inteligente. |
| 3306 | MySQL | Base de datos MySQL. |
| 3389 | RDP | Escritorio remoto de Windows. |
| 5000 | UPnP | Lo usan algunos routers y dispositivos NAS. |
| 5353 | mDNS | Descubrimiento de nombres en la red local (Bonjour). |
| 8000, 8008, 8080, 8888 | HTTP alternativo | Páginas web en un segundo puerto. |
| 8443 | HTTPS alternativo | Páginas web cifradas en un segundo puerto. |
| 9100 | Impresora | Impresión directa en muchas impresoras de red. |

Los números de puerto van del 1 al 65535. Los puertos del 1 al 1023 se llaman puertos bien conocidos.

## Cómo leer el resultado

- Abierto. Un servicio respondió a la conexión.
- Cerrado o filtrado. Nadie respondió, o un cortafuegos descartó la conexión. Un escaneo no siempre distingue ambos casos.
- La mayoría de los puertos abiertos no son un problema. Una impresora en el 631 o el 9100 y una cámara en el 554 son normales.
- Busca puertos inesperados. Si Telnet (23) está abierto en un router o una cámara, revisa los ajustes o actualiza el firmware. Lo mismo vale para SMB (445) en un dispositivo que no debería compartir archivos.
- Redirige un puerto a internet solo si sabes por qué. Si no lo configuraste tú, no debería ser accesible desde fuera.

### Ejemplo

Escaneas un enchufe inteligente y un NAS de la misma red.

1. El enchufe muestra el 80 abierto. Su app usa una pequeña página web, así que es normal.
2. El NAS muestra 22, 80, 443 y 445 abiertos: SSH, administración web y archivos compartidos. Es normal en un NAS.
3. El NAS muestra también el 23 abierto. Telnet casi nunca hace falta. Desactívalo en los ajustes del NAS y vuelve a escanear para confirmar que está cerrado.

## Cómo funciona un escaneo TCP connect

El escáner intenta abrir una conexión TCP normal con cada puerto. Si la conexión se establece, el puerto está abierto. No envía tráfico dañino, pero el dispositivo y cualquier cortafuegos intermedio lo ven. Por eso debes escanear solo tu propia red y los dispositivos que tengas permiso para probar. Escanear la red de otra persona puede ser delito según el país.

## Escanea tu propia red con la app

La pantalla Tools de Escáner WiFi y herramientas tiene un escaneo de puertos con tres ajustes predefinidos y tu propia lista:

| Ajuste | Puertos |
|---|---|
| Common | 24 puertos de la tabla anterior (todos menos el 8008 y el 8888) |
| Web | 7 puertos: 80, 443, 8000, 8008, 8080, 8443, 8888 |
| 1–1024 | Puertos del 1 al 1024 |

También puedes escribir tus propios puertos, como `22,80,443` o `1-1024`. Una ejecución admite hasta 1024 puertos, del 1 al 65535. La herramienta apunta por defecto a tu red local y pide confirmación antes de escanear una dirección pública.

Para encontrar un dispositivo que escanear, haz primero un escaneo en la pantalla Devices. La app muestra cada dispositivo que responde en tu red IPv4 /24, como 192.168.1.0/24, con su nombre y fabricante cuando los encuentra. Abre uno y usa su dirección en el escaneo de puertos. Los resultados se quedan en tu teléfono.

## Comprobaciones relacionadas

- Ping indica si el dispositivo responde y cuánto tarda. Si se bloquea ICMP, la app usa una comprobación TCP.
- La consulta DNS devuelve registros A, AAAA y PTR inverso para un nombre o una dirección.
- Traceroute muestra los saltos entre tu teléfono y un destino.
