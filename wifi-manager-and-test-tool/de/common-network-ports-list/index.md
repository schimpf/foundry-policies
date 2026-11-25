# Häufige Netzwerk-Ports: Liste und Bedeutung

> Liste häufiger TCP-Ports im Heimnetz, wofür jeder Dienst da ist und wie du in deinem eigenen WLAN prüfst, welche Ports ein Gerät offen hat.

- Web: https://apps.schimpf.es/wifi-manager-and-test-tool/de/common-network-ports-list/
- App: WLAN-Scanner & Netzwerktools, https://apps.schimpf.es/wifi-manager-and-test-tool/de/index.md
Ein Port ist eine Nummer, die einem Gerät sagt, für welchen Dienst eine Netzwerkverbindung gedacht ist. Wenn du ein Gerät scannst, bedeutet ein offener Port, dass dort ein Dienst lauscht. Diese Seite listet Ports, die in Heimnetzen und kleinen Büros oft vorkommen, und erklärt, wie du ein Scan-Ergebnis liest.

Portnamen und -nummern stammen aus dem IANA Service Name and Transport Protocol Port Number Registry. Einige Ports in der Liste unten, etwa 5000 und 9100, werden eher aus Gewohnheit als per Registrierung genutzt.

## Häufige Ports

| Port | Dienst | Wofür er da ist |
|---|---|---|
| 21 | FTP | Dateiübertragung. Unverschlüsselt. |
| 22 | SSH | Verschlüsselte Fernanmeldung und Dateikopie. |
| 23 | Telnet | Alte Fernanmeldung. Unverschlüsselt. |
| 25 | SMTP | E-Mail-Versand zwischen Servern. |
| 53 | DNS | Namensauflösung. Router antworten hier oft. |
| 80 | HTTP | Webseiten, auch viele Admin-Seiten von Routern und Kameras. |
| 110 | POP3 | E-Mails abrufen. Unverschlüsselt. |
| 139 | NetBIOS | Windows-Namens- und Dateifreigabe, älter. |
| 143 | IMAP | E-Mails abrufen. Unverschlüsselt. |
| 443 | HTTPS | Verschlüsselte Webseiten. |
| 445 | SMB | Windows- und Samba-Dateifreigabe. |
| 554 | RTSP | Videostreams von IP-Kameras. |
| 631 | IPP | Netzwerkdruck. |
| 993 | IMAPS | IMAP über TLS. |
| 995 | POP3S | POP3 über TLS. |
| 1883 | MQTT | Nachrichten zwischen Smart-Home-Geräten. |
| 3306 | MySQL | MySQL-Datenbank. |
| 3389 | RDP | Windows-Remotedesktop. |
| 5000 | UPnP | Wird von manchen Routern und NAS-Geräten genutzt. |
| 5353 | mDNS | Namenserkennung im lokalen Netz (Bonjour). |
| 8000, 8008, 8080, 8888 | HTTP alternativ | Webseiten auf einem zweiten Port. |
| 8443 | HTTPS alternativ | Verschlüsselte Webseiten auf einem zweiten Port. |
| 9100 | Drucker | Direktdruck auf vielen Netzwerkdruckern. |

Portnummern reichen von 1 bis 65535. Die Ports 1 bis 1023 heißen Well-Known-Ports.

## So liest du das Ergebnis

- Offen. Ein Dienst hat die Verbindung angenommen.
- Geschlossen oder gefiltert. Nichts hat geantwortet, oder eine Firewall hat die Anfrage verworfen. Ein Scan kann das nicht immer unterscheiden.
- Die meisten offenen Ports sind harmlos. Ein Drucker auf 631 oder 9100 und eine Kamera auf 554 sind normal.
- Achte auf unerwartete Ports. Ist Telnet (23) auf einem Router oder einer Kamera offen, prüfe die Einstellungen oder aktualisiere die Firmware. Das gilt auch für SMB (445) auf einem Gerät, das keine Dateien freigeben soll.
- Leite einen Port nur dann ins Internet weiter, wenn du den Grund kennst. Hast du ihn nicht selbst eingerichtet, sollte er von außen nicht erreichbar sein.

### Beispiel

Du scannst eine smarte Steckdose und ein NAS im selben Netz.

1. Die Steckdose zeigt Port 80 offen. Ihre App nutzt eine kleine Webseite, das ist normal.
2. Das NAS zeigt 22, 80, 443 und 445 offen: SSH, Web-Oberfläche und Dateifreigabe. Das ist für ein NAS normal.
3. Das NAS zeigt außerdem 23 offen. Telnet wird selten gebraucht. Schalte es in den NAS-Einstellungen ab und scanne danach erneut, um zu prüfen, dass der Port zu ist.

## So funktioniert ein TCP-Connect-Scan

Der Scanner versucht, zu jedem Port eine normale TCP-Verbindung aufzubauen. Klappt das, ist der Port offen. Er sendet keinen schädlichen Datenverkehr, ist aber für das Gerät und jede Firewall dazwischen sichtbar. Deshalb solltest du nur dein eigenes Netz und Geräte scannen, die du testen darfst. Das Scannen fremder Netze kann je nach Land strafbar sein.

## Dein eigenes Netz mit der App scannen

Der Bildschirm Tools in WLAN-Scanner & Netzwerktools hat einen Port-Scan mit drei Voreinstellungen und deiner eigenen Liste:

| Voreinstellung | Ports |
|---|---|
| Common | 24 Ports aus der Tabelle oben (alle außer 8008 und 8888) |
| Web | 7 Ports: 80, 443, 8000, 8008, 8080, 8443, 8888 |
| 1–1024 | Ports 1 bis 1024 |

Du kannst auch eigene Ports eingeben, etwa `22,80,443` oder `1-1024`. Ein Durchlauf nimmt bis zu 1024 Ports von 1 bis 65535. Das Tool zielt standardmäßig auf dein lokales Netz und fragt nach, bevor es eine öffentliche Adresse scannt.

Um ein Gerät zum Scannen zu finden, starte zuerst einen Scan im Bildschirm Devices. Die App listet jedes Gerät auf, das in deinem IPv4-/24-Netz antwortet, zum Beispiel 192.168.1.0/24, mit Name und Hersteller, soweit sie diese finden kann. Öffne ein Gerät und nutze seine Adresse im Port-Scan. Die Ergebnisse bleiben auf deinem Handy.

## Verwandte Prüfungen

- Ping zeigt, ob das Gerät überhaupt antwortet und wie lange das dauert. Ist ICMP blockiert, nutzt die App stattdessen einen TCP-Test.
- Die DNS-Abfrage liefert A-, AAAA- und PTR-Einträge (Rückwärtsauflösung) für einen Namen oder eine Adresse.
- Traceroute zeigt die Zwischenstationen zwischen deinem Handy und einem Ziel.
