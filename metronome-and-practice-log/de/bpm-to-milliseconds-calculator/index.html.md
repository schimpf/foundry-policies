# BPM in Millisekunden umrechnen: Rechner und Formel

> BPM in Millisekunden pro Schlag umrechnen: eine Formel, Rechenbeispiele und eine Tabelle der Notenlängen von der ganzen Note bis zum Sechzehntel.

- Web: https://apps.schimpf.es/metronome-and-practice-log/de/bpm-to-milliseconds-calculator/
- App: Metronom & Übungsprotokoll, https://apps.schimpf.es/metronome-and-practice-log/de/index.md
Delay-Zeiten, Clicktracks und tempo-synchrone Effekte verlangen oft Millisekunden, während Musik in Schlägen pro Minute (BPM) notiert ist. Die Umrechnung ist eine einzige Division.

## Die Formel

Eine Minute hat 60.000 Millisekunden. Teile sie durch die Anzahl der Schläge, die in dieser Minute liegen:

**Millisekunden pro Schlag = 60.000 / BPM**

Und in die andere Richtung:

**BPM = 60.000 / Millisekunden pro Schlag**

## Rechner

An interactive calculator is on the web page: https://apps.schimpf.es/metronome-and-practice-log/de/bpm-to-milliseconds-calculator/

## Rechenbeispiel

Du übst mit 90 BPM und willst den Abstand zwischen den Klicks wissen.

1. Schreib die Formel auf: 60.000 / 90.
2. Teile: 666,67.
3. Der Abstand zwischen den Schlägen beträgt etwa 667 ms.

Probe: 90 Schläge zu je 666,67 ms ergeben 60.000 ms, also eine Minute.

## Gängige Tempi

| BPM | ms pro Schlag |
|---|---|
| 40 | 1500 |
| 60 | 1000 |
| 72 | 833,3 |
| 80 | 750 |
| 100 | 600 |
| 120 | 500 |
| 144 | 416,7 |
| 180 | 333,3 |
| 240 | 250 |
| 300 | 200 |

```
 60 BPM |##########  1000 ms
120 BPM |#####       500 ms
240 BPM |###         250 ms
```

Doppeltes BPM halbiert den Abstand.

## Notenlängen bei einem Tempo

Die BPM-Zahl zählt eine Art Schlag, meist die Viertelnote. Andere Notenwerte sind Bruchteile davon. Bei 100 BPM, mit der Viertelnote als Schlag (600 ms):

| Note | Anteil an einer Viertelnote | Länge bei 100 BPM |
|---|---|---|
| Ganze | 4 | 2400 ms |
| Halbe | 2 | 1200 ms |
| Viertel | 1 | 600 ms |
| Achtel | 1/2 | 300 ms |
| Achteltriole | 1/3 | 200 ms |
| Sechzehntel | 1/4 | 150 ms |

Für jeden dieser Werte rechnest du die Viertelnote mit der Formel aus und multiplizierst mit dem Anteil. Eine punktierte Note ist 1,5-mal so lang wie die einfache. Eine punktierte Viertelnote bei 100 BPM dauert 600 x 1,5 = 900 ms.

## Was als Schlag zählt

Achte darauf, wenn der Schlag keine Viertelnote ist. Im 6/8-Takt kann eine Partitur die punktierte Viertelnote als Schlag angeben, das ergibt zwei Schläge pro Takt. Klickt ein Metronom stattdessen jede Achtelnote, ist das eingestellte BPM die Zahl der Achtelnoten pro Minute und damit dreimal so hoch wie das Tempo der punktierten Viertel. Eine punktierte Viertel bei 60 BPM entspricht Achteln bei 180 BPM.

Metronom & Übungsprotokoll folgt derselben Regel: Das eingestellte BPM ist die Zahl der Klicks pro Minute, und jeder Schlag des Takts bekommt einen Klick. Im 6/8-Takt sind das sechs Klicks pro Takt. Standardmäßig betont die App den ersten und den vierten Klick, du hörst also zwei Pulse der punktierten Viertel. Die Betonung kannst du bei jedem Schlag ändern.

## Warum die Timing-Genauigkeit zählt

Bei 120 BPM dauert ein Schlag 500 ms. Ein Fehler von 10 ms sind 2 Prozent des Schlags, und Fehler von gewöhnlichen Timern summieren sich über einen Takt oder zwei. Smartphone-Metronome, die sie nutzen, können wandern, besonders bei ausgeschaltetem Bildschirm.

Die App zählt Audio-Samples statt Timer. Jeder Schlag wird mit seiner genauen Länge an die Audioausgabe geschrieben, und der Nachkommaanteil der Länge wandert in den nächsten Schlag, damit das Tempo nicht driftet. Bei 48.000 Samples pro Sekunde und 100 BPM hat ein Schlag zum Beispiel 28.800 Samples, eine exakte Zahl. Bei 70 BPM sind es 41.142,857 Samples, und der Rest wird weitergegeben, sodass der Durchschnitt genau bei 70 BPM bleibt. Tempoänderungen gelten ab dem nächsten Schlag.

## Runden

- Für Delay-Plugins rundest du auf ganze Millisekunden. Der Fehler liegt unter einer halben Millisekunde.
- Für Clicktracks behältst du zwei Nachkommastellen, wenn das Programm es erlaubt.
- Runde nicht das BPM. 666,67 ms entsprechen 90 BPM, 667 ms ergeben dagegen 89,96 BPM.

## In der App ausprobieren

Metronom & Übungsprotokoll ist ein Android-Metronom, das offline arbeitet und jede Übungseinheit automatisch protokolliert. Es läuft von 30 bis 300 BPM, das sind 2000 ms bis 200 ms pro Schlag. Es hält den Takt im Hintergrund und bei ausgeschaltetem Bildschirm und bietet Bildschirmblitz und Vibration auf dem Schlag. Such die App bei Google Play.
