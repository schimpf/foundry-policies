# Tinag2: Icinga & Nagios Alarme

> Icinga-2- und Nagios-Probleme im Blick, bestätigen und Alarme erhalten.

- Android-App, Gerrit Schimpf
- Web: https://apps.schimpf.es/tinag2/de/
- Bald bei Google Play
- Datenschutz: https://apps.schimpf.es/tinag2/privacy/
- Tools
- Kontakt: apps@schimpf.es
- EN: https://apps.schimpf.es/tinag2/index.md
- ES: https://apps.schimpf.es/tinag2/es/index.md

## Über die App

Tinag2 ist ein Android-Client für Icinga 2 und Nagios/Naemon (über Thruk). Sieh, was ausgefallen ist, reagiere darauf und lass dich benachrichtigen, direkt auf dem Smartphone.

Verbinde deine eigenen Monitoring-Server. Du kannst beliebig viele hinzufügen; sie werden parallel abgefragt. Die App spricht nur mit den Servern, die du selbst einträgst. Es gibt kein Konto und keinen Server des Entwicklers.

## Funktionen

### Übersicht

- Anzahl kritischer Probleme, Warnungen, unbekannter Zustände und ausgefallener Hosts
- Karte "Needs you now" für unbearbeitete Probleme
- Anzeige der Servicegesundheit und eine Karte pro Server
- Zeigt das Alter der Daten und behält die letzten guten Daten, wenn ein Server nicht erreichbar ist

### Probleme

- Eine Liste nach Dringlichkeit sortiert: unbearbeitete zuerst, schlimmster Zustand zuerst, älteste zuerst
- Filter für unbearbeitet, kritisch, Warnung und harte Zustände
- Suche per Text oder regulärem Ausdruck
- Services auf ausgefallenen Hosts sind standardmäßig ausgeblendet
- Bestätigte Probleme und Probleme in Wartungszeit erscheinen gedämpft
- Nach rechts wischen zum Bestätigen, nach links für einen erneuten Check. Dieselben Aktionen gibt es als Bedienungshilfen-Aktionen.
- Detailansicht mit Zustand, Prüfversuchen, Ausgabe sowie letztem und nächstem Check
- Wartungszeit von einer Stunde setzen

### Alarme

- Benachrichtigt nur bei neuen oder schlimmer gewordenen Problemen
- Die Benachrichtigung verschwindet, wenn das Problem behoben oder bearbeitet ist
- Regeln: Warnungen an oder aus, weiche Zustände überspringen, bestätigte überspringen, Wartungszeit überspringen, 5 Minuten vor dem Alarm warten
- Ruhezeit von 22:00 bis 07:00, optional mit Ausnahme für kritische Alarme
- Eigene Benachrichtigungskanäle für kritisch und Host down, Warnungen, unbekannt und Verbindungsprobleme
- Direkt aus der Benachrichtigung bestätigen

### Widgets

- Zähler-Widget mit Anzahl kritisch, Warnung und unbekannt
- Listen-Widget mit den dringendsten unbearbeiteten Problemen

### Verbindung und sicherheit

- Icinga-2-REST-API und Thruk-REST-API
- HTTP-Basic-Authentifizierung
- Optionales Pinning des Zertifikat-Fingerabdrucks, für selbstsignierte Server
- Passwörter werden mit dem Android Keystore verschlüsselt
- Einfaches HTTP ist für lokale Netze erlaubt; die App warnt dich dabei
- Keine Werbung, keine Analyse, kein Tracking

### Details

Tinag2 braucht einen Icinga-2- oder Thruk-Server, den du vom Smartphone aus erreichen kannst.

- Hintergrundabgleich alle 15 Minuten sowie Aktualisieren per Herunterziehen
- Helles und dunkles Design nach Systemeinstellung
- Auf dem Smartphone untere Navigation, auf Tablets Listen- und Detailansicht

## Screenshots

- [Screenshot 1](https://apps.schimpf.es/tinag2/screen-1.png)
- [Screenshot 2](https://apps.schimpf.es/tinag2/screen-2.png)
- [Screenshot 3](https://apps.schimpf.es/tinag2/screen-3.png)
- [Screenshot 4](https://apps.schimpf.es/tinag2/screen-4.png)

## Ratgeber

- [Selbstsigniertes Icinga-Zertifikat: SHA-256-Fingerabdruck](https://apps.schimpf.es/tinag2/de/icinga-self-signed-certificate-fingerprint/index.md): So liest du den SHA-256-Fingerabdruck des selbstsignierten Zertifikats von Icinga 2 oder Thruk mit openssl aus und trägst ihn in der App ein.
- [Nagios und Icinga: Soft State und Hard State erklärt](https://apps.schimpf.es/tinag2/de/nagios-soft-vs-hard-states-explained/index.md): Was Soft State und Hard State in Nagios und Icinga 2 bedeuten, wie Prüfversuche zählen und wie lange ein Ausfall bis zum Hard State braucht.

## Häufige Fragen

### Was kann Tinag2?

Tinag2 zeigt dir die aktuellen Probleme deiner Icinga-2- und Nagios/Naemon-Server (über Thruk), nach Dringlichkeit sortiert. Du kannst ein Problem bestätigen, einen erneuten Check anfordern, eine Wartungszeit von einer Stunde setzen und wirst bei neuen oder schlimmer gewordenen Problemen benachrichtigt.

### Was kann Tinag2 nicht?

Die App prüft höchstens alle 15 Minuten auf neue Probleme, weil es keinen Push-Dienst gibt. Sie unterstützt nur Icinga 2 und Thruk, meldet sich nur mit Benutzername und Passwort an (keine Client-Zertifikate) und hat keine Wear-OS-App.

### Wo bleiben meine Daten?

Auf deinem Smartphone. Die App spricht nur mit den Servern, die du einträgst. Es gibt keinen Server des Entwicklers, kein Konto, keine Analyse und keine Werbung. Passwörter werden mit dem Android Keystore verschlüsselt.

### Muss ich etwas kaufen?

Nein. Die App hat keine Käufe und keine Werbung. Du brauchst einen eigenen Icinga-2- oder Thruk-Server, den dein Smartphone erreicht.

### Welche Android-Versionen werden unterstützt?

Android 8.0 oder neuer.

### Funktioniert Tinag2 mit einem selbstsignierten Zertifikat?

Ja. Füge den SHA-256-Fingerabdruck des Serverzertifikats in den Einstellungen der Instanz ein, dann akzeptiert die App dieses Zertifikat. Ohne Fingerabdruck muss das Zertifikat die normale Android-Prüfung bestehen.
