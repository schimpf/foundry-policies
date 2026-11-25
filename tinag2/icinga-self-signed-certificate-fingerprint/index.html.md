# SHA-256 fingerprint of a self-signed Icinga certificate

> How to read the SHA-256 fingerprint of an Icinga 2 or Thruk server certificate with openssl, and how to use it to connect a mobile app safely.

- Web: https://apps.schimpf.es/tinag2/icinga-self-signed-certificate-fingerprint/
- App: Tinag2: Icinga & Nagios Alerts, https://apps.schimpf.es/tinag2/index.md
Many Icinga 2 servers use a self-signed certificate. A phone does not trust it, so connections fail. The safe fix is to pin the certificate, which means you give the client the exact SHA-256 fingerprint to accept, and leave certificate checks on. This page shows how to read that fingerprint and what to check before you trust it.

## What a fingerprint is

A certificate fingerprint is a hash of the certificate file in its binary (DER) form. SHA-256 gives 32 bytes, shown as 64 hex characters, often in pairs separated by colons:

`3A:9F:...:C1` (32 pairs)

Two different certificates do not share a fingerprint. If the server certificate is replaced, the fingerprint changes.

## Get the fingerprint with openssl

You need a computer that can reach the server and has OpenSSL installed.

1. Pick the host name and port. The Icinga 2 API listens on port 5665 by default (Icinga 2 documentation, chapter "Icinga 2 API"). Thruk and most web front ends use port 443.
2. Run this command, with your own host name and port:

```
openssl s_client -connect icinga.example.com:5665 -servername icinga.example.com </dev/null 2>/dev/null | openssl x509 -noout -fingerprint -sha256
```

3. The output looks like this:

```
sha256 Fingerprint=3A:9F:12:...:C1
```

4. Copy the part after the equals sign.

The command takes the first certificate the server presents, which is the server's own (leaf) certificate. That is the one to pin.

## Check it before you trust it

Reading the fingerprint over the network trusts whatever answered. On an untrusted network, someone could answer in place of your server. To be sure:

- Run the command from a trusted network, ideally the server's own LAN or from the server itself.
- Or compare with the certificate file on the server. For Icinga 2 the API certificate is in the Icinga 2 data directory (commonly `/var/lib/icinga2/certs/`). Run `openssl x509 -in <file> -noout -fingerprint -sha256` on it and compare the two values.

## Use the fingerprint in Tinag2

Tinag2 is an Android client for Icinga 2 and Nagios/Naemon through Thruk. Each server you add can have an optional certificate pin.

1. Open **Instances** and tap **Add instance**, or edit an existing one.
2. Enter the name, type, URL, user and password.
3. Paste the fingerprint into the field "Trusted certificate SHA-256 (optional)".
4. Save and refresh.

The app compares the fingerprint with the SHA-256 of the certificate the server presents. It ignores colons and upper or lower case, so you can paste the openssl output as it is, minus the `sha256 Fingerprint=` prefix.

## What pinning does and does not do

- The server's leaf certificate is accepted if its fingerprint matches your pin. Any other certificate must pass the normal system checks.
- With a pin set, the app does not require the host name in the certificate to match. The fingerprint identifies the server instead. This helps when you connect by IP address or an internal name that the certificate does not list.
- The pin applies to that one server only. Other servers in the app keep their own settings.
- Plain HTTP is also allowed for local networks. The instance dialog warns you when you use it, because passwords sent over HTTP are readable on the network. A pinned HTTPS connection is better.

## When the connection fails after it worked

The most common cause is a new certificate. Icinga 2 and Thruk certificates expire, and a renewed or regenerated certificate has a new fingerprint. Run the openssl command again and update the pin.

Other causes:

- Login rejected (HTTP 401 or 403): the user name or password is wrong, or the API user lacks permission.
- API not found (HTTP 404): the base URL is wrong. For Icinga 2 use the API address with port, such as `https://icinga.example.com:5665`. For Thruk use the Thruk root, such as `https://mon.example.com/thruk`.
- Can't reach the host: the phone is not on a network that can reach the server, for example a VPN is off.

Tinag2 shows the problems on your Icinga 2 or Thruk server, lets you acknowledge, recheck and set downtime, and notifies you about new or worse problems. Your passwords are encrypted with the Android Keystore, and the app talks only to the servers you enter.
