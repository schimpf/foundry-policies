# BPM in ms Tabelle für Hardtechno, 140 bis 220 BPM

> Millisekunden pro Viertel, Achtel, Sechzehntel und Takt für 140 bis 220 BPM, mit Formeln und Rechenbeispiel zur Songlänge in Sekunden.

- Web: https://apps.schimpf.es/tekkno-rave-daw/de/bpm-to-ms-chart/
- App: Tekkno Rave DAW: Beat-Maker, https://apps.schimpf.es/tekkno-rave-daw/de/index.md
Delay-Zeiten, Loop-Längen und Sample-Schnitte gehen leichter von der Hand, wenn du weißt, wie viele Millisekunden ein Schlag dauert. Diese Seite enthält eine Tabelle für den Tempobereich von Hardtechno und Hardcore (140 bis 220 BPM), die Formeln dahinter und einen kleinen Rechner.

## Die Formeln

BPM steht für Beats per Minute, also Schläge pro Minute. Eine Minute hat 60.000 Millisekunden, deshalb gilt:

- Schlag (Viertelnote) in ms = 60000 / BPM
- Achtelnote in ms = 30000 / BPM
- Sechzehntelnote in ms = 15000 / BPM
- Takt (4/4) in ms = 240000 / BPM

Ein 4/4-Takt hat 4 Schläge, das sind 16 Sechzehntelnoten. Die meisten Step-Sequencer, auch ein Pattern mit 16 Schritten, behandeln einen Schritt als eine Sechzehntelnote.

## BPM in ms Tabelle

| BPM | Sechzehntel (ms) | Achtel (ms) | Viertel (ms) | Takt (ms) |
|-----|------------------|-------------|--------------|-----------|
| 140 | 107,14 | 214,29 | 428,57 | 1714,29 |
| 150 | 100,00 | 200,00 | 400,00 | 1600,00 |
| 160 | 93,75 | 187,50 | 375,00 | 1500,00 |
| 170 | 88,24 | 176,47 | 352,94 | 1411,76 |
| 175 | 85,71 | 171,43 | 342,86 | 1371,43 |
| 180 | 83,33 | 166,67 | 333,33 | 1333,33 |
| 190 | 78,95 | 157,89 | 315,79 | 1263,16 |
| 200 | 75,00 | 150,00 | 300,00 | 1200,00 |
| 210 | 71,43 | 142,86 | 285,71 | 1142,86 |
| 220 | 68,18 | 136,36 | 272,73 | 1090,91 |

Die Werte sind auf zwei Nachkommastellen gerundet.

## Rechenbeispiel: Wie lang ist mein Track?

Angenommen, dein Track hat 175 BPM und 32 Takte.

1. Ein Takt bei 175 BPM = 240000 / 175 = 1371,43 ms.
2. 32 Takte = 32 x 1371,43 = 43.885,7 ms.
3. Das sind rund 43,9 Sekunden.

Zur Kontrolle: 32 Takte x 16 Schritte = 512 Schritte. Ein Schritt bei 175 BPM = 15000 / 175 = 85,71 ms. 512 x 85,71 = 43.885,7 ms. Das Ergebnis ist dasselbe.

Längere Tracks wachsen linear: 64 Takte bei 175 BPM dauern rund 87,8 Sekunden, 128 Takte rund 175,5 Sekunden.

## Von Millisekunden zu Audio-Frames

Digitales Audio wird in Frames gezählt. Bei einer Abtastrate von 44,1 kHz sind es 44.100 Frames pro Sekunde.

Frames pro Sechzehntel = 44100 x 60 / BPM / 4

Bei 175 BPM sind das 44100 x 60 / 175 / 4 = 3.780 Frames pro Schritt. Ein Tempo, das sich so glatt teilen lässt, hält die Schritte auf ganzen Frames. Bei 170 BPM kommen 3.891,18 Frames heraus, deshalb muss ein Sequencer die Position mit Nachkommastellen mitführen, um in einem langen Loop im Takt zu bleiben.

## Welches Tempo für welchen Stil?

Tempobereiche sind lose Konventionen. Genre-Namen überlappen sich, und Produzenten sprengen die Bereiche ständig. Als grobe Richtschnur:

- Hardtechno liegt oft bei etwa 150 bis 160 BPM.
- Gabber und Hardcore liegen oft bei etwa 170 bis 200 BPM.
- Speedcore geht noch höher.

Die Tabelle oben deckt 140 bis 220 BPM ab, den Bereich der Tempo-Regelung in der App.

## Tipps zum Arbeiten mit den Werten

- Für eine Delay-Zeit, die im Raster liegt, nimm den Achtel- oder Sechzehntelwert aus der Tabelle. Eine punktierte Achtel ist das 1,5-Fache des Achtelwerts.
- Eine Kick auf jedem Schlag bei 175 BPM wiederholt sich alle 342,86 ms. Das sind 175 Kicks pro Minute.
- Höheres Tempo verkürzt jeden Schritt. Samples, die länger klingen als ein Schritt, überlappen den nächsten Treffer. Kürze lange Kicks und Bass-Tails, wenn du die BPM erhöhst.
- Ein Tempowechsel ändert in einem Step-Sequencer die Tonhöhe nicht. Es ändert sich nur der Abstand zwischen den Auslösern.

## Rechner

An interactive calculator is on the web page: https://apps.schimpf.es/tekkno-rave-daw/de/bpm-to-ms-chart/

## In der App ausprobieren

Tekkno Rave DAW ist eine Android-Groovebox für Hardtechno und Hardcore. Das Tempo reicht von 140 bis 220 BPM, ein Pattern hat 8, 16, 32 oder 64 Schritte, und ein Schritt ist eine Sechzehntelnote. In der Song-Ansicht besteht ein Takt aus 16 Schritten, die Formel für die Songlänge oben ist also die, die die App bei der Wiedergabe verwendet.
