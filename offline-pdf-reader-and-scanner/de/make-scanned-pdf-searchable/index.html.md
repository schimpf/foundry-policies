# Gescanntes PDF durchsuchbar machen (Android, OCR)

> Warum ein gescanntes PDF keine Suche zulässt, wie OCR eine Textebene ergänzt und wie du einen Scan auf dem Handy durchsuchbar machst.

- Web: https://apps.schimpf.es/offline-pdf-reader-and-scanner/de/make-scanned-pdf-searchable/
- App: PDF-Reader & Scanner, https://apps.schimpf.es/offline-pdf-reader-and-scanner/de/index.md
Du scannst einen Vertrag, öffnest ihn, suchst nach einem Wort und bekommst „Keine Treffer“. Die Seite zeigt Wörter, doch die Datei enthält nur ein Bild davon. Diese Seite erklärt, warum das so ist, wie du es prüfst und wie du es auf Android behebst, ohne die Datei irgendwohin hochzuladen.

## Warum ein gescanntes PDF keinen durchsuchbaren Text hat

Eine PDF-Seite kann zwei Arten von Inhalt enthalten:

- **Textobjekte.** Echte Zeichen mit Schriftart und Position. Suchen, Kopieren und Markieren funktionieren damit.
- **Bilder.** Ein Foto der Seite. Deine Augen lesen die Wörter, die Datei enthält aber keine Zeichen.

Ein Kamerascan besteht nur aus einem Bild. Ein PDF aus Word oder von einer Webseite enthält meist echten Text. Deshalb scheitert die Suche bei Scans und funktioniert bei Dokumenten vom Computer.

## So prüfst du, ob dein PDF eine Textebene hat

1. Öffne das PDF in einem Reader.
2. Suche nach einem Wort, das du auf der Seite siehst.
3. Versuche, eine Zeile mit langem Drücken zu markieren.

Findet die Suche nichts und lässt sich kein Text markieren, besteht die Seite nur aus einem Bild.

## Was OCR macht

OCR steht für optische Zeichenerkennung (englisch: optical character recognition). Die Software betrachtet das Bild, findet Textzeilen und ermittelt, welche Zeichen darin stehen. Diese Zeichen schreibt sie als unsichtbare Ebene über das Bild in das PDF.

- Die Seite sieht genauso aus wie vorher.
- Suchen, Kopieren und Markieren funktionieren jetzt auf der Seite.
- Das Originalbild bleibt in der Datei.

Die Genauigkeit hängt vom Scan ab. Scharfe, glatte, gut beleuchtete Seiten mit Druckschrift liefern die besten Ergebnisse. Unscharfe Fotos, Schatten, Handschrift und ungewöhnliche Schriftarten führen zu mehr Fehlern.

## Scan durchsuchbar machen mit Offline PDF reader and scanner

Die App führt die Texterkennung auf deinem Handy aus, mit dem mitgelieferten Latein-Modell von Google ML Kit. Es wird nichts hochgeladen, und die App hat keine Internetberechtigung. Die Texterkennung ist eine Pro-Funktion (Einmalkauf).

### Variante 1: automatisch nach jedem Scan

1. Öffne die **Einstellungen** und prüfe, ob **Scans durchsuchbar machen** aktiviert ist. Nach dem Freischalten von Pro ist die Option standardmäßig an.
2. Tippe auf dem Startbildschirm auf **Dokument scannen**.
3. Scanne die Seiten und tippe auf **Scan speichern**.
4. Nach dem Speichern startet die Texterkennung. Den Fortschritt siehst du in der Zeile des Scans in der Bibliothek.

Das Ergebnis ersetzt den Scan, du behältst also eine Datei pro Scan.

### Variante 2: ein PDF, das du schon hast

1. Öffne das reine Bild-PDF im Reader.
2. Suche nach einem Wort. Die App meldet, dass keine Textebene vorhanden ist, und fragt, ob sie das PDF durchsuchbar machen soll.
3. Bestätige. Die App startet die Texterkennung.

Bei einem importierten PDF speichert die App das Ergebnis als Kopie in der Bibliothek mit dem Zusatz „(durchsuchbar)“. Die Originaldatei bleibt unverändert.

### Variante 3: nach dem Hinzufügen von Seiten

Wenn du im Seiteneditor Seiten zu einem gespeicherten Scan hinzufügst, erhalten die neuen Seiten ebenfalls Texterkennung. Beim Speichern wird der Scan ersetzt.

## Was bei der Erkennung passiert

- Jede Seite wird mit 2480 Pixeln Breite gerendert. Bei einer A4-Seite sind das etwa 300 dpi, eine übliche Auflösung für OCR.
- Das Modell für das lateinische Alphabet liest jede Seite und liefert Textzeilen mit ihren Positionen.
- Die App schreibt alle Zeilen als unsichtbaren Text ins PDF und ersetzt danach die Datei einmalig.
- Die Erkennung läuft als normale Hintergrundarbeit. Du kannst die App verlassen, während sie arbeitet.
- Dauert sie länger als 30 Minuten oder schlägt sie fehl, markiert die App den Scan als fehlgeschlagen. Die Datei bleibt, wie sie war.

Lange Dokumente brauchen länger, weil jede Seite einzeln verarbeitet wird.

## Grenzen

- **Nur lateinisches Alphabet.** Deutsch, Englisch, Spanisch und andere Sprachen mit lateinischen Buchstaben funktionieren. Kyrillisch, Griechisch, Arabisch, Chinesisch, Japanisch und Koreanisch werden nicht unterstützt.
- **Nur mit Pro.** Lesen, einfaches Scannen und die Suche in PDFs, die schon Text enthalten, brauchen kein Pro.
- **Google Play-Dienste.** Scannen und Pro brauchen sie. Das Lesen von PDFs funktioniert auch ohne.
- **Wichtige Zahlen prüfen.** OCR kann eine 5 als 6 lesen. Vergleiche Beträge, Daten und Nummern mit der Seite.

## Nach der Erkennung: suchen und markieren

Sobald eine Seite eine Textebene hat, kannst du:

1. Im Reader auf das Suchsymbol tippen und ein Wort eingeben.
2. Mit den Schaltflächen „Weiter“ und „Zurück“ zwischen den Treffern springen.
3. Text lange drücken und ziehen, um ihn zu markieren. Markierungen sind normale PDF-Anmerkungen, deshalb zeigen auch andere Reader sie an. Die App speichert sie als Kopie in deiner Bibliothek und ändert das Original nie.

## Fragen

### Wird die Datei durch OCR größer?

Etwas. Die Textebene ist klein im Vergleich zu den Seitenbildern.

### Kann ich vor der OCR suchen?

Nein. Ohne Textebene gibt es nichts zu durchsuchen. Starte zuerst die Texterkennung.

### Wird mein Scan an einen Server gesendet?

Nein. Die Erkennung läuft auf dem Handy, und die App hat keine Internetberechtigung.

## Ausprobieren

Offline PDF reader and scanner gibt es bei Google Play. Scanne eine Seite, warte, bis die Erkennung fertig ist, und suche ein Wort darauf.
