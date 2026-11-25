# Binaurale Beats berechnen: Frequenz-Rechner und Formel

> Berechne den linken und rechten Ton für jeden binauralen Beat mit Formel, Rechenbeispiel und Rechner. Mit Verlauf des Beats über die Zeit.

- Web: https://apps.schimpf.es/binaural-beats/de/binaural-beat-frequency-calculator/
- App: Binaural Beats, https://apps.schimpf.es/binaural-beats/de/index.md
Ein binauraler Beat entsteht aus zwei reinen Tönen, einem pro Ohr. Der Beat, den du wahrnimmst, ist der Unterschied zwischen beiden. Diese Seite zeigt die Formel, ein Rechenbeispiel und einen Rechner. Danach geht es darum, einen Beat von einer Frequenz zur nächsten gleiten zu lassen.

## Die Formel für binaurale Beats

- Ton links = Trägerfrequenz
- Ton rechts = Trägerfrequenz + Beat-Frequenz
- Beat-Frequenz = Ton rechts − Ton links

Alle Werte sind in Hertz (Hz). Der Träger ist der Grundton, den du tatsächlich hörst. Der Beat ist der langsame Puls, den du aus dem Unterschied wahrnimmst.

So arbeitet auch die App Binaural Beats: Links liegt der Träger, rechts der Träger plus Beat.

## Rechenbeispiel

Du willst einen 10-Hz-Beat auf einem 400-Hz-Träger.

1. Linkes Ohr: 400 Hz.
2. Rechtes Ohr: 400 + 10 = 410 Hz.
3. Probe: 410 − 400 = 10 Hz, du nimmst also 10 Schläge pro Sekunde wahr.

Bei 10 Hz liegt der Beat im Alpha-Bereich (8 bis unter 12 Hz). Die Standard-Vorlage der App, Ruhiger Fokus, nutzt genau diese Zahlen.

Noch ein Beispiel: Ein 4-Hz-Beat auf einem 250-Hz-Träger ergibt 250 Hz links und 254 Hz rechts. 4 Hz gehören zu Theta (4 bis unter 8 Hz).

## Rechner

An interactive calculator is on the web page: https://apps.schimpf.es/binaural-beats/de/binaural-beat-frequency-calculator/

## Die Zahlen wählen

### Trägerfrequenz

Binaurale Beats nutzen meist Träger unter etwa 1000 Hz. Die App akzeptiert 100 bis 1000 Hz und empfiehlt 200 bis 500 Hz als angenehmen Bereich. Tiefe Träger klingen dunkler, hohe heller. Der Träger bestimmt den Ton, den du hörst, und lässt die Beat-Frequenz unverändert.

### Beat-Frequenz

Die App akzeptiert 0,25 bis 45 Hz. Über etwa 30 Hz sind binaurale Beats schwer wahrzunehmen. Bei höheren Werten schlägt die App deshalb einen monauralen oder isochronen Beat vor.

| Beat (Hz) | Bereich |
|---|---|
| unter 4 | Delta |
| 4 bis unter 8 | Theta |
| 8 bis unter 12 | Alpha |
| 12 bis unter 30 | Beta |
| 30 und mehr | Gamma |

### Kopfhörer

Ein binauraler Beat entsteht nur, wenn jedes Ohr seinen eigenen Ton hört. Nimm Stereo-Kopfhörer oder In-Ear-Kopfhörer. Über Lautsprecher mischen sich die beiden Töne in der Luft, und du hörst stattdessen einen monauralen Beat. Das ist ein anderer Effekt, aber ebenfalls ein echter Puls.

## Andere Beat-Arten, gleiche Beat-Frequenz

Die Beat-Frequenz bedeutet in allen vier Modi dasselbe:

- **Monaural:** Beide Töne, Träger und Träger plus Beat, werden addiert und auf beide Ohren gespielt. Der Puls steckt im Klang.
- **Isochron:** Ein Ton auf der Trägerfrequenz, der im Takt des Beats ein- und ausgeschaltet wird.
- **Bilateral:** Ein Ton auf der Trägerfrequenz, der pro Beat-Zyklus einmal zwischen den Ohren wechselt.

Bei isochronen und bilateralen Beats kann der Puls eine weiche Sinusform oder ein weiches Rechteck mit schärferen Kanten haben.

## Einen Beat über die Zeit gleiten lassen

Eine Sitzung aus mehreren Schritten kann den Beat nach und nach ändern. Die App lässt die Frequenz auf einer geometrischen Skala gleiten: Jeder gleich lange Zeitabschnitt multipliziert die Frequenz mit demselben Faktor.

Formel: Beat zum Zeitpunkt t = Start × (Ende ÷ Start)^t, wobei t im Schritt von 0 bis 1 läuft.

Rechenbeispiel: Ein Schritt gleitet von 12 Hz auf 6 Hz.

1. In der Mitte ist t = 0,5.
2. Das Verhältnis Ende ÷ Start = 6 ÷ 12 = 0,5.
3. 0,5 hoch 0,5 ergibt etwa 0,707.
4. Beat = 12 × 0,707 ≈ 8,49 Hz.

Ein gerader, linearer Verlauf läge in der Mitte bei 9 Hz. Die geometrische Variante verbringt gleich viel Zeit mit jeder Verdopplung oder Halbierung, also dauert 12 auf 6 Hz genauso lange wie 6 auf 3 Hz. Aus diesem Grund ist auch der Beat-Regler in der App logarithmisch.

Sind beide Enden eines Schritts gleich, bleibt der Beat konstant. Nach dem letzten Schritt bleiben die Endwerte bis zum Ende der Sitzung bestehen.

## Was die Forschung sagt

Die Belege dafür, dass binaurale Beats Stimmung, Fokus oder Schlaf verändern, sind uneinheitlich. Die Metaanalyse von Garcia-Argibay, Santed und Reales aus dem Jahr 2019 („Efficacy of binaural auditory beats in cognition, anxiety, and pain perception: a meta-analysis“, Psychological Research) fand kleine bis moderate Effekte, mit großen Unterschieden zwischen den Studien. Sieh Beats als Entspannungshilfe. Halte die Lautstärke niedrig und hör nicht beim Autofahren. Frag vorher deine Ärztin oder deinen Arzt, wenn du Epilepsie, einen Herzschrittmacher oder eine andere Erkrankung hast.

## In der App ausprobieren

Binaural Beats für Android erzeugt diese Töne live, du kannst also jeden Träger und Beat aus den Beispielen oben testen.

1. Wähle den Modus Binaural, stelle Träger und Beat ein und lies die Anzeige des Frequenzbereichs ab.
2. Füge auf Wunsch weißes, rosa oder braunes Rauschen mit eigener Lautstärke hinzu.
3. Starte eine Sitzung von 5 bis 90 Minuten oder baue eine Sitzung aus Schritten und sieh den Beat in einem Diagramm.

Die App spielt im Hintergrund, mit Steuerung auf dem Sperrbildschirm, und funktioniert offline. Du kannst eine Sitzung auch als WAV-Datei speichern.
