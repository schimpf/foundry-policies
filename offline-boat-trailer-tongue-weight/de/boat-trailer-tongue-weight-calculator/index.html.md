# Stützlast Bootstrailer berechnen: Formel und Rechner

> Stützlast deines Bootstrailers aus Gewicht und Position der Ladung berechnen. Formel, Beispiel, Zielwert 7 bis 10 Prozent und ein kleiner Rechner.

- Web: https://apps.schimpf.es/offline-boat-trailer-tongue-weight/de/boat-trailer-tongue-weight-calculator/
- App: Bootstrailer Stützlast, https://apps.schimpf.es/offline-boat-trailer-tongue-weight/de/index.md
Die Stützlast ist die Kraft, mit der die Kupplung des Trailers nach unten auf die Kugel drückt. Bei einem Bootstrailer liegt der übliche Zielwert bei 7 bis 10 Prozent des Gesamtgewichts des Trailers. Diese Seite zeigt, wie du sie aus Gewicht und Position jedes Postens auf dem Trailer schätzt, mit einem Rechenbeispiel und einem Rechner, den du direkt hier benutzen kannst.

## Was die Stützlast ist

Der Trailer ruht auf seiner Achse (oder seinen Achsen) und auf der Zugkugel. Was die Achse nicht trägt, trägt die Kupplung. Dieser Anteil ist die Stützlast.

- Zu wenig (unter etwa 5 Prozent) und der Trailer kann schlingern.
- Zu viel (über etwa 15 Prozent) und das Heck des Zugfahrzeugs sackt ab, die Front hebt sich, und Lenkung und Bremsen leiden.
- 7 bis 10 Prozent ist der übliche Zielwert für Bootstrailer.

Der Bereich von 7 bis 10 Prozent ist eine verbreitete Faustregel und kein gesetzlicher Grenzwert. Trailer- und Kupplungshersteller können einen anderen Bereich nennen, also lies die Handbücher. Die harte Grenze ist die maximale Stützlast auf dem Schild von Kupplung und Aufnahme.

## Die Formel

Die Schätzung ist ein Momentengleichgewicht um die Trailerachse. Miss jede Position in Zentimetern von der Achse. Eine Position Richtung Kupplung ist positiv. Eine Position Richtung Heck ist negativ.

1. Moment jedes Postens = Gewicht x Position von der Achse.
2. Gesamtmoment = Summe aller Postenmomente plus das Moment des leeren Trailers.
3. Stützlast = Gesamtmoment / Abstand von der Kupplung zur Achse.
4. Stützlast in Prozent = Stützlast / Gesamtgewicht des Trailers x 100.

Das Gesamtgewicht des Trailers ist der leere Trailer plus alles, was darauf liegt. Bei einem Tandemtrailer misst du bis zur Mitte zwischen den beiden Achsen.

### Der leere Trailer

Auch der nackte Rahmen hat ein Gewicht und einen Schwerpunkt. Kennst du ihn nicht, ist eine brauchbare Annahme, dass der Rahmen bei 20 Prozent des Abstands von Kupplung zur Achse vor der Achse im Gleichgewicht ist. Der Rechner unten nutzt diesen Wert, solange du ihn nicht änderst.

## Rechenbeispiel

Nimm einen Tandemtrailer mit 420 cm Abstand von der Kupplung zur Achse.

| Posten | Gewicht (kg) | Position von der Achse (cm) | Moment (kg·cm) |
| --- | --- | --- | --- |
| Leerer Trailer | 550 | +84 (20 % von 420) | 46.200 |
| Rumpf | 800 | +75 | 60.000 |
| Außenbordmotor | 180 | -230 | -41.400 |
| Kraftstoff, 150 l Benzin | 110 | -100 | -11.000 |
| Ausrüstung | 70 | +50 | 3.500 |
| **Summe** | **1.710** | | **57.300** |

- Stützlast = 57.300 / 420 = 136,4 kg
- Stützlast in Prozent = 136,4 / 1.710 = 8,0 Prozent

Das liegt im Zielbereich von 7 bis 10 Prozent.

Zur Kraftstoffzeile: 150 Liter Benzin zu 0,73 kg pro Liter sind etwa 110 kg. Die Gewichte anderer Flüssigkeiten findest du unter [Gewicht von Benzin, Diesel und Wasser pro Liter](/de/boat-fuel-and-water-weight-per-gallon).

### Achslast im selben Beispiel

Die Achsen tragen alles außer der Stützlast: 1.710 - 136,4 = 1.573,6 kg. Bei einem Tandemtrailer sind das etwa 786,8 kg pro Achse. Vergleiche das mit der Achslast auf dem Typenschild des Trailers. Die App zeigt Warn, sobald eine Last 90 Prozent einer Angabe erreicht.

## Rechner

An interactive calculator is on the web page: https://apps.schimpf.es/offline-boat-trailer-tongue-weight/de/boat-trailer-tongue-weight-calculator/

## Das Ergebnis lesen

So liest du den Prozentwert:

| Stützlast in Prozent | Bedeutung |
| --- | --- |
| Unter 5 | Zu leicht, Schlingergefahr |
| 5 bis unter 7 | Leicht, anpassen, wenn möglich |
| 7 bis 10 | Zielwert |
| Über 10 bis 15 | Schwer, anpassen, wenn möglich |
| Über 15 | Zu schwer |

Prüfe außerdem die Stützlast gegen das Maximum auf dem Schild von Kupplung und Aufnahme und das volle Trailergewicht gegen die Anhängelast deines Fahrzeugs und das zulässige Gesamtgewicht des Trailers.

## Genauigkeit

Das ist eine Schätzung. Sie ist nur so gut wie die Gewichte und Abstände, die du eingibst.

- Nimm echte Gewichte aus Datenblättern oder von einer Waage.
- Miss jede Position bis zum Schwerpunkt des Postens. Beim Rumpf ist der schwer zu kennen, deshalb ist der Rumpfwert die schwächste Eingabe.
- Flüssigkeiten bewegen sich. Kraftstoff und Wasser ändern beim Verbrauch Gewicht und Gleichgewicht.
- Wiege das beladene Gespann im Zweifel auf einer geeichten Waage, auch wenn das Ergebnis nah an einer Grenze liegt.

Liegt das Ergebnis außerhalb von 7 bis 10 Prozent, findest du unter [Stützlast am Bootstrailer erhöhen](/de/how-to-increase-boat-trailer-tongue-weight), wie du es behebst.

## In der App

Die Android-App Boat Trailer Tongue Weight rechnet das für dein ganzes Gespann. Du gibst die Werte von Türaufkleber, Kupplungsschild und Typenschild des Trailers ein und fügst dann Rumpf, Motor, Kraftstoff, Wasser und Ausrüstung mit ihren Positionen hinzu. Sie zeigt den leeren und den beladenen Trailer nebeneinander, bewertet jede Angabe als Pass, Warn oder Fail und schlägt Änderungen für 7 bis 10 Prozent vor. Sie läuft offline, also auch an der Slipanlage. Die App lässt sich auf metrische Einheiten umstellen, die Oberfläche ist auf Englisch.

Diese Seite und die App sind Planungshilfen und ersetzen keine geeichte Waage. Du bist für eine sichere und legale Fahrt verantwortlich.
