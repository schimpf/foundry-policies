# Selbstsigniertes Icinga-Zertifikat: SHA-256-Fingerabdruck

> So liest du den SHA-256-Fingerabdruck des selbstsignierten Zertifikats von Icinga 2 oder Thruk mit openssl aus und trägst ihn in der App ein.

- Web: https://apps.schimpf.es/tinag2/de/icinga-self-signed-certificate-fingerprint/
- App: Tinag2: Icinga & Nagios Alarme, https://apps.schimpf.es/tinag2/de/index.md
Viele Icinga-2-Server nutzen ein selbstsigniertes Zertifikat. Das Smartphone vertraut ihm nicht, deshalb schlagen Verbindungen fehl. Die sichere Lösung ist, das Zertifikat zu pinnen: Du gibst dem Client den genauen SHA-256-Fingerabdruck, den er akzeptieren soll, und lässt die Zertifikatsprüfung eingeschaltet. Diese Seite zeigt, wie du den Fingerabdruck ausliest und was du prüfst, bevor du ihm vertraust.

## Was ein Fingerabdruck ist

Der Fingerabdruck eines Zertifikats ist ein Hash der Zertifikatsdatei in ihrer binären Form (DER). SHA-256 liefert 32 Bytes, dargestellt als 64 Hex-Zeichen, oft paarweise durch Doppelpunkte getrennt:

`3A:9F:...:C1` (32 Paare)

Zwei verschiedene Zertifikate haben nie denselben Fingerabdruck. Wird das Serverzertifikat ersetzt, ändert sich der Fingerabdruck.

## Fingerabdruck mit openssl auslesen

Du brauchst einen Rechner, der den Server erreicht und auf dem OpenSSL installiert ist.

1. Wähle Hostname und Port. Die Icinga-2-API lauscht standardmäßig auf Port 5665 (Icinga-2-Dokumentation, Kapitel "Icinga 2 API"). Thruk und die meisten Web-Oberflächen nutzen Port 443.
2. Führe diesen Befehl mit deinem eigenen Hostnamen und Port aus:

```
openssl s_client -connect icinga.example.com:5665 -servername icinga.example.com </dev/null 2>/dev/null | openssl x509 -noout -fingerprint -sha256
```

3. Die Ausgabe sieht so aus:

```
sha256 Fingerprint=3A:9F:12:...:C1
```

4. Kopiere den Teil nach dem Gleichheitszeichen.

Der Befehl nimmt das erste Zertifikat, das der Server sendet. Das ist das eigene Zertifikat des Servers (Leaf-Zertifikat) und genau das, was du pinnen willst.

## Vor dem Vertrauen prüfen

Wer den Fingerabdruck über das Netzwerk liest, vertraut dem, was geantwortet hat. In einem nicht vertrauenswürdigen Netz könnte jemand anstelle deines Servers antworten. So gehst du sicher:

- Führe den Befehl in einem vertrauenswürdigen Netz aus, am besten im LAN des Servers oder direkt auf dem Server.
- Oder vergleiche mit der Zertifikatsdatei auf dem Server. Bei Icinga 2 liegt das API-Zertifikat im Datenverzeichnis von Icinga 2 (meist `/var/lib/icinga2/certs/`). Führe darauf `openssl x509 -in <Datei> -noout -fingerprint -sha256` aus und vergleiche beide Werte.

## Fingerabdruck in Tinag2 eintragen

Tinag2 ist ein Android-Client für Icinga 2 und für Nagios/Naemon über Thruk. Für jeden Server, den du hinzufügst, kannst du optional einen Zertifikat-Pin setzen.

1. Öffne **Instances** und tippe auf **Add instance**, oder bearbeite eine vorhandene.
2. Gib Name, Typ, URL, Benutzer und Passwort ein.
3. Füge den Fingerabdruck in das Feld "Trusted certificate SHA-256 (optional)" ein.
4. Speichere und aktualisiere.

Die App vergleicht den Fingerabdruck mit dem SHA-256 des Zertifikats, das der Server sendet. Sie ignoriert Doppelpunkte sowie Groß- und Kleinschreibung. Du kannst die openssl-Ausgabe also unverändert einfügen, ohne das Präfix `sha256 Fingerprint=`.

## Was Pinning leistet und was nicht

- Das Leaf-Zertifikat des Servers wird akzeptiert, wenn sein Fingerabdruck zu deinem Pin passt. Jedes andere Zertifikat muss die normale Systemprüfung bestehen.
- Mit gesetztem Pin verlangt die App nicht, dass der Hostname im Zertifikat passt. Der Fingerabdruck identifiziert den Server. Das hilft, wenn du dich per IP-Adresse oder mit einem internen Namen verbindest, den das Zertifikat nicht enthält.
- Der Pin gilt nur für diesen einen Server. Andere Server in der App behalten ihre eigenen Einstellungen.
- Einfaches HTTP ist für lokale Netze ebenfalls erlaubt. Der Instanz-Dialog warnt dich dabei, weil Passwörter über HTTP im Netz mitgelesen werden können. Eine gepinnte HTTPS-Verbindung ist besser.

## Wenn die Verbindung nach einer funktionierenden Phase scheitert

Die häufigste Ursache ist ein neues Zertifikat. Zertifikate von Icinga 2 und Thruk laufen ab, und ein erneuertes oder neu erzeugtes Zertifikat hat einen neuen Fingerabdruck. Führe den openssl-Befehl erneut aus und aktualisiere den Pin.

Weitere Ursachen:

- Anmeldung abgelehnt (HTTP 401 oder 403): Benutzername oder Passwort stimmen nicht, oder dem API-Benutzer fehlt die Berechtigung.
- API nicht gefunden (HTTP 404): Die Basis-URL stimmt nicht. Für Icinga 2 nimmst du die API-Adresse mit Port, etwa `https://icinga.example.com:5665`. Für Thruk nimmst du das Thruk-Stammverzeichnis, etwa `https://mon.example.com/thruk`.
- Host nicht erreichbar: Das Smartphone ist in keinem Netz, das den Server erreicht, zum Beispiel weil das VPN aus ist.

Tinag2 zeigt die Probleme deines Icinga-2- oder Thruk-Servers, lässt dich bestätigen, erneut prüfen und eine Wartungszeit setzen und benachrichtigt dich bei neuen oder schlimmer gewordenen Problemen. Deine Passwörter werden mit dem Android Keystore verschlüsselt, und die App spricht nur mit den Servern, die du einträgst.
