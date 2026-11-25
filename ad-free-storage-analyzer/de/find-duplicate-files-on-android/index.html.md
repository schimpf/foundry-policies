# Doppelte Dateien auf Android finden und löschen

> Doppelte Dateien auf dem Android-Handy finden: wie eine SHA-256-Prüfsumme echte Kopien beweist und welche Kopie du beim Löschen behältst.

- Web: https://apps.schimpf.es/ad-free-storage-analyzer/de/find-duplicate-files-on-android/
- App: Speicheranalyse: Große Dateien, https://apps.schimpf.es/ad-free-storage-analyzer/de/index.md
Doppelte Dateien füllen den Speicher unbemerkt. Dasselbe Video liegt zweimal auf dem Handy, ein Download wurde wiederholt oder ein Foto steckt in zwei Ordnern. Diese Seite zeigt, wie du exakte Duplikate findest, wie du sicher bist, dass es echte Kopien sind, und wie du sie löschst, ohne etwas zu verlieren.

## Was ein Duplikat ist

Ein exaktes Duplikat hat denselben Inhalt, Byte für Byte. Name, Ordner und Datum können abweichen. Zwei Fotos, die nur ähnlich aussehen, sind keine exakten Duplikate, weil sich ihre Bytes unterscheiden.

Der Name taugt nicht als Merkmal. Zwei Dateien namens `IMG_0042.jpg` können verschiedene Fotos sein, und ein Video, das als `clip.mp4` und `clip (1).mp4` gespeichert ist, ist dieselbe Datei unter zwei Namen. Entscheidend ist der Inhalt.

## Schritt für Schritt: Duplikate von Hand finden

1. Öffne eine Dateimanager-App und geh in den Ordner, den du verdächtigst, zum Beispiel Download.
2. Sortiere nach Größe, die größte zuerst.
3. Suche Dateien mit exakt gleicher Größe in Bytes. Die genaue Zahl steht in den Dateidetails.
4. Öffne beide Dateien und vergleiche sie.
5. Lösche die Kopie, die du nicht brauchst.

Das klappt bei ein paar Dateien. Bei Hunderten wird es langsam. Außerdem beweist gleiche Größe nicht, dass zwei Dateien identisch sind, denn verschiedene Dateien können gleich groß sein.

## Wie eine Prüfsumme beweist, dass zwei Dateien gleich sind

Eine Prüfsumme ist ein kurzer Fingerabdruck, der aus jedem Byte einer Datei berechnet wird. SHA-256 ist eine genormte Hashfunktion (NIST, *FIPS PUB 180-4: Secure Hash Standard*, 2015). Sie liefert ein Ergebnis aus 64 Zeichen, zum Beispiel `9f86d081…`.

- Identische Dateien ergeben immer dieselbe SHA-256-Summe.
- Weicht ein einziges Byte ab, ist das Ergebnis völlig anders.
- Dass zwei verschiedene Dateien dieselbe Summe ergeben, spielt in der Praxis keine Rolle.

Jedes Byte einer großen Datei zu lesen dauert, deshalb arbeitet ein guter Scanner in zwei Schritten:

1. **Nach Größe gruppieren.** Eine Datei, deren Größe keine andere hat, kann kein Duplikat sein. Sie wird übersprungen.
2. **Nur die Gruppen hashen.** Dateien gleicher Größe bekommen eine SHA-256-Summe über die ganze Datei. Gleiches Ergebnis heißt exakte Kopie.

### Rechenbeispiel

Auf deinem Handy liegen diese Dateien:

| Datei | Größe |
|---|---|
| `urlaub.mp4` | 48.201.330 Bytes |
| `urlaub (1).mp4` | 48.201.330 Bytes |
| `vorlesung.mp4` | 48.201.330 Bytes |
| `notizen.pdf` | 2.310.004 Bytes |

1. `notizen.pdf` hat eine einmalige Größe und wird übersprungen.
2. Die drei Videos sind gleich groß, deshalb bekommt jedes eine SHA-256-Summe.
3. `urlaub.mp4` und `urlaub (1).mp4` ergeben dasselbe Ergebnis. `vorlesung.mp4` ergibt ein anderes.
4. Ergebnis: eine Duplikatgruppe mit zwei Dateien. Wenn du eine Kopie löschst, werden 48.201.330 Bytes frei, etwa 48,2 MB.

## Welche Kopie du behältst

Behalte die neueste Kopie. Sie hast du am ehesten mit Absicht bearbeitet oder verschoben, ältere Kopien sind meist Überbleibsel. Haben zwei Kopien dasselbe Datum, ist es egal, welche du behältst, denn der Inhalt ist gleich.

Behalte immer mindestens eine Kopie pro Gruppe. Wenn du alle löschst, ist die Datei weg.

## Duplikate mit Storage Analyzer finden

Storage Analyzer sucht exakte Duplikate, nachdem du auf Scan getippt hast. Die App ist nur auf Englisch verfügbar, deshalb stehen die Bezeichnungen hier so, wie du sie in der App siehst. Sie geht nach den zwei Schritten von oben vor:

- Geprüft werden nur Dateien ab 1 MB (1.000.000 Bytes). Kleine Dateien bringen wenig Platz.
- Dateien gleicher Größe werden per SHA-256 über die ganze Datei verglichen. Es erscheinen nur echte Kopien.
- Die Gruppen sind nach dem Platzgewinn sortiert, die größte zuerst.
- Die neueste Kopie ist vorausgewählt zum Behalten. Du kannst die Auswahl für jede Datei ändern.
- Mindestens eine Kopie bleibt immer erhalten.
- Eine Datei, die die App nicht lesen kann, fehlt in den Ergebnissen. Sie zählt nicht als Kopie.

Gelöschte Dateien landen im Papierkorb (Trash) der App. Du kannst direkt danach rückgängig machen oder sie 7 Tage lang aus dem Papierkorb wiederherstellen. Danach sind sie endgültig gelöscht. Die Dateien werden auf demselben Speicher verschoben und nicht kopiert, das geht auch bei großen Videos schnell. Beim Deinstallieren der App wird ihr Papierkorb geleert, stelle also vorher wieder her, was du behalten willst.

Die App findet nur exakte Duplikate. Ähnliche Fotos erkennt sie nicht.

## Kurze Checkliste

- Gleiche Größe und dann gleiche Prüfsumme heißt gleiche Datei.
- Behalte die neueste Kopie.
- Prüfe die Gruppe, bevor du löschst.
- Lösche zuerst in den Papierkorb und leere ihn später.
