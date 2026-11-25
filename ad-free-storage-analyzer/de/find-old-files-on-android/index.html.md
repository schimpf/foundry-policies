# Alte Dateien auf Android finden und aufräumen

> Dateien finden, die seit über 90 Tagen unverändert sind: alte Downloads, Screenshots, WhatsApp-Medien und APK-Installer. Mit Regeln und Beispiel.

- Web: https://apps.schimpf.es/ad-free-storage-analyzer/de/find-old-files-on-android/
- App: Speicheranalyse: Große Dateien, https://apps.schimpf.es/ad-free-storage-analyzer/de/index.md
Alte Dateien sammeln sich an ein paar vorhersehbaren Stellen. Downloads, die du einmal geöffnet hast, Screenshots, die du nicht mehr brauchst, Medien aus Chats und Installationsdateien für Apps, die längst installiert sind. Diese Seite erklärt, wo du suchst, was „alt“ heißen kann und wie du sicher aufräumst.

## Was „alt“ bedeutet

Eine Datei ist alt, wenn sie sich eine bestimmte Zeit lang nicht geändert hat. Android speichert für jede Datei ein Datum der letzten Änderung. Storage Analyzer nennt eine Datei alt, wenn dieses Datum mehr als 90 Tage zurückliegt.

Die Regel in Zahlen: 90 Tage × 24 Stunden × 60 Minuten × 60 Sekunden × 1.000 Millisekunden = 7.776.000.000 ms. Eine Datei ist alt, wenn jetzt minus letzte Änderung größer ist als dieser Wert.

### Rechenbeispiel

Heute ist der 1. November. Prüfe drei Dateien:

| Datei | Letzte Änderung | Tage her | Alt? |
|---|---|---|---|
| `rechnung.pdf` | 15. Juli | 109 | Ja |
| `setup.apk` | 10. September | 52 | Nein |
| `meme.jpg` | 3. August | 90 | Nein, genau 90 ist nicht mehr als 90 |

„Letzte Änderung“ ist nicht „zuletzt geöffnet“. Eine Datei, die du oft öffnest, ist trotzdem alt, wenn du sie nie änderst.

## Wo sich alte Dateien verstecken

### Downloads

Browser und Apps speichern hier standardmäßig. Das ist der erste Ordner, den du prüfen solltest.

### Screenshots

Screenshots entstehen für einen Moment und werden selten wieder gebraucht. Oft liegen sie in einem Ordner namens Screenshots.

### WhatsApp-Medien

Fotos, Videos und Sprachnachrichten aus Chats liegen in den WhatsApp-Ordnern. Sie können über ein Jahr hinweg sehr groß werden.

### APK-Installer

Eine APK ist die Installationsdatei einer App. Ist die App installiert, braucht man die Datei meist nicht mehr.

## Schritt für Schritt: von Hand aufräumen

1. Öffne eine Dateimanager-App und geh in den Ordner Download.
2. Sortiere nach Datum, die älteste zuerst.
3. Prüfe Dateien, die älter als 90 Tage sind. Lösche, was du nicht brauchst.
4. Wiederhole das für den Ordner Screenshots, die WhatsApp-Ordner und jeden Ordner mit APK-Dateien.
5. Bevor du ein Dokument löschst, das du vielleicht noch brauchst, kopiere es an einen sicheren Ort.

## Alte Dateien mit Storage Analyzer finden

Nach deinem Tipp auf Scan gruppiert die App alte Dateien für dich. Sie ist nur auf Englisch verfügbar, deshalb stehen die Gruppennamen so da, wie du sie in der App siehst:

- **Downloads:** alte Dateien im obersten Ordner Download oder Downloads.
- **Screenshots:** alte Dateien in jedem Ordner namens Screenshots.
- **WhatsApp media:** alte Dateien in WhatsApp-Ordnern, auch bei WhatsApp Business.
- **APK installers:** alte Installationsdateien (APK, APKS, XAPK und APKM), außer sie liegen in Download-, Screenshots- oder WhatsApp-Ordnern. Dann gehören sie in diese Gruppe.
- **Other old files:** alles andere, was alt ist.

„Other old files“ lässt deine eigenen Foto-, Video- und Musikordner aus: DCIM, Pictures, Movies, Music, Recordings, Podcasts und Audiobooks. Ein altes Urlaubsfoto ist kein Datenmüll. Willst du diese Dateien trotzdem prüfen, nutze die Liste der großen Dateien.

Der Startbildschirm zeigt eine freigebbare Größe. Sie addiert alte Dateien, APK-Installer und jede Duplikatkopie außer der neuesten. Große Dateien zählen nicht mit, weil eine große Datei an sich noch kein Datenmüll ist.

## Ohne Risiko löschen

- Gelöschte Dateien landen im Papierkorb (Trash) der App. Mach sofort rückgängig oder stelle sie innerhalb von 7 Tagen aus dem Papierkorb wieder her.
- Nach 7 Tagen sind die Dateien endgültig gelöscht. Die Prüfung läuft beim Start der App und einmal am Tag.
- Dateien werden verschoben und nicht kopiert, deshalb geht das Löschen schnell.
- Ordner werden nie gelöscht, nur Dateien.
- Beim Deinstallieren der App wird auch ihr Papierkorb geleert, stelle also vorher wieder her, was du behalten willst.

## Scans laufen nur von Hand

Die App scannt nur, wenn du auf Scan tippst. Im Hintergrund scannt sie nie. Im vollen Modus nutzt sie den Zugriff auf alle Dateien und prüft jeden Ordner im internen Speicher und auf der SD-Karte. Im eingeschränkten Modus sieht sie nur die Fotos, Videos und Musik, die Android mit Apps teilt, deshalb ist die Liste der alten Dateien kürzer.

## Kurze Checkliste

- Alt heißt: mehr als 90 Tage seit der letzten Änderung.
- Prüfe zuerst Downloads, Screenshots, WhatsApp-Medien und APK-Dateien.
- Lass persönliche Fotos und Musik aus dem Datenmüll heraus.
- Lösche zuerst in den Papierkorb und leere ihn später.
