# Tinag2: Alertas Icinga/Nagios

> Vigila problemas de Icinga 2 y Nagios, reconócelos y recibe alertas.

- app para Android, Gerrit Schimpf
- Web: https://apps.schimpf.es/tinag2/es/
- Pronto en Google Play
- Privacidad: https://apps.schimpf.es/tinag2/privacy/
- Tools
- Contacto: apps@schimpf.es
- EN: https://apps.schimpf.es/tinag2/index.md
- DE: https://apps.schimpf.es/tinag2/de/index.md

## Acerca de la app

Tinag2 es un cliente Android para Icinga 2 y Nagios/Naemon (a través de Thruk). Mira qué falla, actúa y recibe avisos, directamente desde el móvil.

Conecta tus propios servidores de monitorización. Puedes añadir todos los que necesites; se consultan en paralelo. La aplicación solo habla con los servidores que tú introduces. No hay cuenta ni servidor del desarrollador.

## Funciones

### Resumen

- Recuento de problemas críticos, avisos, desconocidos y hosts caídos
- Tarjeta "Needs you now" para los problemas sin atender
- Barra de salud de los servicios y una tarjeta por servidor
- Muestra la antigüedad de los datos y conserva los últimos datos buenos si un servidor no responde

### Problemas

- Una lista ordenada por urgencia: primero los sin atender, primero el peor estado, primero los más antiguos
- Filtros para sin atender, críticos, avisos y estados duros
- Búsqueda por texto o expresión regular
- Los servicios de un host caído se ocultan por defecto
- Los problemas reconocidos o en mantenimiento se muestran atenuados
- Desliza a la derecha para reconocer y a la izquierda para volver a comprobar. Las mismas acciones están disponibles como acciones de accesibilidad.
- Vista de detalle con estado, intentos de comprobación, salida, última y próxima comprobación
- Programa un mantenimiento de una hora

### Alertas

- Avisa solo de problemas nuevos o que han empeorado
- El aviso desaparece cuando el problema se recupera o se atiende
- Reglas: avisos activados o no, omitir estados blandos, omitir reconocidos, omitir mantenimiento, esperar 5 minutos antes de alertar
- Horas de silencio de 22:00 a 07:00, con opción de dejar pasar las alertas críticas
- Canales de notificación separados para críticos y host caído, avisos, desconocidos y problemas de conexión
- Reconoce directamente desde la notificación

### Widgets

- Un widget de recuentos con críticos, avisos y desconocidos
- Un widget de lista con los problemas sin atender más urgentes

### Conexión y seguridad

- API REST de Icinga 2 y API REST de Thruk
- Autenticación básica HTTP
- Fijación opcional de la huella del certificado, para servidores con certificado propio
- Las contraseñas se cifran con el Android Keystore
- Se permite HTTP sin cifrar en redes locales, y la aplicación te avisa
- Sin anuncios, sin analítica, sin rastreo

### Detalles

Tinag2 necesita un servidor Icinga 2 o Thruk al que puedas acceder desde el móvil.

- Sincronización en segundo plano cada 15 minutos y actualización al deslizar
- Tema claro y oscuro según el sistema
- Navegación inferior en el móvil y vista de lista y detalle en tabletas

## Capturas

- [Screenshot 1](https://apps.schimpf.es/tinag2/screen-1.png)
- [Screenshot 2](https://apps.schimpf.es/tinag2/screen-2.png)
- [Screenshot 3](https://apps.schimpf.es/tinag2/screen-3.png)
- [Screenshot 4](https://apps.schimpf.es/tinag2/screen-4.png)

## Guías

- [Huella SHA-256 de un certificado autofirmado de Icinga](https://apps.schimpf.es/tinag2/es/icinga-self-signed-certificate-fingerprint/index.md): Cómo obtener con openssl la huella SHA-256 (fingerprint) del certificado autofirmado de un servidor Icinga 2 o Thruk y usarla en la app Android.
- [Estados soft y hard en Nagios e Icinga explicados](https://apps.schimpf.es/tinag2/es/nagios-soft-vs-hard-states-explained/index.md): Qué significan los estados soft y hard en Nagios e Icinga 2, cómo cuentan los intentos de comprobación y cuánto tarda un fallo en ser hard.

## Preguntas frecuentes

### ¿Qué hace Tinag2?

Tinag2 muestra los problemas actuales de tus servidores Icinga 2 y Nagios/Naemon (a través de Thruk), ordenados por urgencia. Puedes reconocer un problema, pedir una nueva comprobación, programar un mantenimiento de una hora y recibir avisos de problemas nuevos o que han empeorado.

### ¿Qué no hace Tinag2?

Busca problemas nuevos cada 15 minutos como máximo, porque no hay servicio push. Solo es compatible con Icinga 2 y Thruk, solo usa usuario y contraseña (sin certificados de cliente) y no tiene aplicación para Wear OS.

### ¿Dónde se quedan mis datos?

En tu móvil. La aplicación solo habla con los servidores que introduces. No hay servidor del desarrollador, ni cuenta, ni analítica, ni anuncios. Las contraseñas se cifran con el Android Keystore.

### ¿Tengo que comprar algo?

No. La aplicación no tiene compras ni anuncios. Necesitas tu propio servidor Icinga 2 o Thruk al que llegue tu móvil.

### ¿Qué versiones de Android son compatibles?

Android 8.0 o posterior.

### ¿Funciona con un certificado autofirmado?

Sí. Pega la huella SHA-256 del certificado del servidor en los ajustes de la instancia y la aplicación aceptará ese certificado. Sin huella, el certificado debe superar la comprobación normal de Android.
