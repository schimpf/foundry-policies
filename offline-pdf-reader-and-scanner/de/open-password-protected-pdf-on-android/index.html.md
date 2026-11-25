# Passwortgeschütztes PDF auf Android öffnen

> Warum ein PDF nach einem Passwort fragt, ab welcher Android-Version es sich öffnen lässt, was bei Fehlern hilft und welche zwei PDF-Passwörter es gibt.

- Web: https://apps.schimpf.es/offline-pdf-reader-and-scanner/de/open-password-protected-pdf-on-android/
- App: PDF-Reader & Scanner, https://apps.schimpf.es/offline-pdf-reader-and-scanner/de/index.md
Du tippst auf ein PDF, und es fragt nach einem Passwort oder lässt sich gar nicht öffnen. Ob es klappt, hängt vom Passwort und von deiner Android-Version ab. Diese Seite behandelt beides.

## Zwei Arten von PDF-Passwörtern

Die PDF-Spezifikation (ISO 32000-1:2008, Abschnitt 7.6, und ISO 32000-2:2020 für PDF 2.0) kennt zwei Passwörter:

| Passwort | Wofür es gilt |
| --- | --- |
| **Benutzerpasswort (Öffnen)** | Nötig, um die Datei zu öffnen und zu lesen. |
| **Besitzerpasswort (Berechtigungen)** | Legt Einschränkungen fest, zum Beispiel kein Drucken oder kein Kopieren. Die Datei öffnet sich auch ohne. |

Ein Reader fragt nur dann nach einem Passwort, wenn die Datei ein Benutzerpasswort hat. Das hat der Absender gewählt. Aus der Datei lässt es sich nicht auslesen, und die App kann ein verlorenes Passwort nicht wiederherstellen.

## Welche Android-Versionen sie öffnen können

In Offline PDF reader and scanner hängt die Antwort vom PDF-Modul des Systems ab:

| Android-Version | Passwortgeschütztes PDF |
| --- | --- |
| Android 15 (API 35) und neuer | Öffnet sich nach Eingabe des Passworts |
| Android 14 (API 34) und älter | Nicht unterstützt. Die App zeigt eine Meldung. |

Auf älteren Versionen zeigt die App „Passwort-PDFs brauchen Android 15“ und erklärt, dass das Gerät sie nicht öffnen kann. Sie rät nicht und versucht auch keinen Umweg.

## So öffnest du eines ab Android 15

1. Öffne das PDF aus deinen Dateien, einem E-Mail-Anhang oder einer Cloud-App. Wähle **Öffnen mit** und dann die App, oder wähle die Datei in der App aus.
2. Ein Dialog zeigt **Passwort erforderlich**.
3. Gib das Passwort ein und tippe auf **Öffnen**.
4. Ist es falsch, meldet die App **Falsches Passwort**. Versuche es noch einmal.

Bei Passwörtern zählt die Groß- und Kleinschreibung. Achte auf ein Leerzeichen am Ende, wenn du es aus einer Nachricht kopiert hast.

## Wenn du das Passwort nicht hast

- Frag den Absender. Banken, Arbeitgeber und Behörden nutzen oft eine feste Regel, etwa das Geburtsdatum oder die Kundennummer. Die E-Mail oder der Brief nennt meist, welche.
- Suche keine Programme zum Knacken von Passwörtern für Dateien, die dir nicht gehören. Viele davon sind unsicher, und das Öffnen fremder geschützter Dateien kann strafbar sein.
- Gehört die Datei dir und das Passwort ist verloren, kann dir die ursprüngliche Quelle (zum Beispiel dein Online-Banking) meist eine neue Kopie geben.

## Wenn es auf einer älteren Android-Version nicht klappt

Du hast drei Möglichkeiten:

1. Aktualisiere das Handy auf Android 15, wenn der Hersteller das anbietet.
2. Öffne die Datei am Computer, wo die meisten PDF-Reader ein Passwort akzeptieren.
3. Bitte den Absender um eine Kopie ohne Benutzerpasswort, falls der Inhalt nicht vertraulich ist.

## Was noch funktioniert, wenn die Datei offen ist

- Kontinuierliches vertikales Scrollen und Weiterlesen auf der letzten Seite.
- Das Inhaltsverzeichnis, falls die Datei eines hat.
- Textsuche, wenn das PDF eine Textebene hat. Bei einem Scan ergänzt die Texterkennung (Pro) eine.
- Nachtseiten, die die Seitenfarben umkehren, um im Dunkeln zu lesen.

Die App merkt sich, wo du aufgehört hast, sodass du später weiterlesen kannst. Die Liste der zuletzt geöffneten Dateien merkt sich nur, wo ein PDF liegt. Die App lädt das Original nicht hoch und ändert es nicht, und du kannst die Liste in den Einstellungen löschen.

## Datenschutz bei geschützten Dateien

Das Öffnen geschieht auf dem Gerät. Die App hat keine Internetberechtigung, deshalb werden weder die Datei noch das eingegebene Passwort irgendwohin gesendet.

## Fragen

### Warum öffnet sich dasselbe PDF im Browser, aber hier nicht?

Manche Browser und Desktop-Reader bringen ein eigenes PDF-Modul mit. Auf Android nutzt die App das System-Modul, das Passwörter ab Android 15 unterstützt.

### Hindert mich das Besitzerpasswort am Lesen?

Nein. Eine Datei mit nur einem Besitzerpasswort öffnet sich ohne Abfrage. Die Einschränkungen betreffen Aktionen wie das Drucken.

### Entfernt die App das Passwort?

Nein. Sie öffnet die Datei nur, damit du sie lesen kannst.

## Ausprobieren

Offline PDF reader and scanner gibt es bei Google Play. Öffne ein geschütztes PDF und gib das Passwort ein.
