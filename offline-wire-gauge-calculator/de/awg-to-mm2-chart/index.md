# AWG in mm² umrechnen: Tabelle mit Querschnitt, Widerstand

> AWG in mm² umrechnen. Tabelle mit Querschnitt, nächster metrischer Größe und Kupferwiderstand, dazu Formel und Rechenbeispiel.

- Web: https://apps.schimpf.es/offline-wire-gauge-calculator/de/awg-to-mm2-chart/
- App: Kabelquerschnitt-Rechner: NEC, https://apps.schimpf.es/offline-wire-gauge-calculator/de/index.md
Eine AWG-Angabe ist eine Stelle auf einer Skala. Je größer die Zahl, desto dünner der Draht. Diese Seite enthält eine Umrechnungstabelle von 18 AWG bis 250 kcmil, die Formel dahinter und einen kleinen Rechner für jede Größe.

## AWG-mm²-Tabelle (Kupfer)

Die Spalte "Nächste Normgröße" nennt den kleinsten metrischen Normquerschnitt, der mindestens so groß ist wie der AWG-Draht. Sie ordnet nur Größen zu und dimensioniert keinen Stromkreis.

| AWG | Querschnitt (mm²) | Nächste Normgröße (mm²) | Ω/km | Ω je 1000 ft |
|---|---|---|---|---|
| 18 | 0,823 | 1 | 20,9 | 6,39 |
| 16 | 1,31 | 1,5 | 13,2 | 4,01 |
| 14 | 2,08 | 2,5 | 8,29 | 2,53 |
| 12 | 3,31 | 4 | 5,21 | 1,59 |
| 10 | 5,26 | 6 | 3,28 | 0,999 |
| 8 | 8,37 | 10 | 2,06 | 0,628 |
| 6 | 13,3 | 16 | 1,30 | 0,395 |
| 4 | 21,2 | 25 | 0,815 | 0,248 |
| 2 | 33,6 | 35 | 0,513 | 0,156 |
| 1/0 | 53,5 | 70 | 0,322 | 0,0983 |
| 2/0 | 67,4 | 70 | 0,256 | 0,0779 |
| 3/0 | 85,0 | 95 | 0,203 | 0,0618 |
| 4/0 | 107 | 120 | 0,161 | 0,0490 |
| 250 kcmil | 127 | 150 | 0,136 | 0,0415 |

Der Widerstand gilt für einen massiven Kupferleiter bei 20 °C. Aluminium hat bei gleicher Größe etwa das 1,64-Fache des Kupferwiderstands, weil seine Leitfähigkeit 61 % der von Kupfer beträgt.

## So funktioniert AWG

Jeder Schritt zu einer kleineren AWG-Zahl macht den Draht dicker. Alle 6 Schritte halbiert sich der Durchmesser ungefähr, alle 3 Schritte verdoppelt sich die Fläche ungefähr. Daraus ergeben sich ein paar Faustregeln:

- 10 AWG hat etwa 5,3 mm². Drei Schritte dicker (7 AWG) wären etwa 10,6 mm², also die doppelte Fläche.
- Von 12 AWG auf 6 AWG vervierfacht sich die Fläche ungefähr (3,31 auf 13,3 mm²).
- Größen über 4/0 werden in kcmil angegeben. Ein kcmil sind 0,5067 mm².

## Die Formel

Der AWG-Durchmesser ist durch eine geometrische Reihe zwischen 36 AWG und 0000 (4/0) AWG festgelegt. Die Norm ASTM B258, *Standard Specification for Standard Nominal Diameters and Cross-Sectional Areas of AWG Sizes of Solid Round Wires Used as Electrical Conductors*, verwendet sie.

1. Durchmesser in mm: d = 0,127 × 92^((36 − n) / 39), wobei n die AWG-Zahl ist. Für 1/0 gilt n = 0, für 2/0 n = −1, für 3/0 n = −2 und für 4/0 n = −3.
2. Fläche in mm²: A = π / 4 × d².
3. Für kcmil-Größen: A = kcmil × 0,5067.
4. Widerstand in Ω/km: ρ / A × 1000, mit ρ = 1/58 Ω·mm²/m für geglühtes Kupfer (100 % IACS, International Annealed Copper Standard) und ρ = (1/58) / 0,61 für Aluminium (61 % IACS).
5. Ω je 1000 ft = Ω/km × 0,3048.

### Rechenbeispiel: 10 AWG Kupfer

1. n = 10, also d = 0,127 × 92^(26 / 39) = 0,127 × 92^0,6667 = 0,127 × 20,38 = 2,588 mm.
2. A = π / 4 × 2,588² = 5,26 mm².
3. Widerstand = (1 / 58) / 5,26 × 1000 = 3,28 Ω/km.
4. In Fuß: 3,28 × 0,3048 = 0,999 Ω je 1000 ft.
5. Die kleinste metrische Größe ab 5,26 mm² ist 6 mm².

## Metrische Größen

Die Spalte "Nächste Normgröße" verwendet die Nennquerschnitte nach IEC 60228, *Conductors of insulated cables*. Sie lauten 0,5, 0,75, 1, 1,5, 2,5, 4, 6, 10, 16, 25, 35, 50, 70, 95, 120, 150, 185, 240, 300, 400, 500, 630, 800 und 1000 mm². AWG- und metrische Größen stimmen selten genau überein. Beim Austausch eines Kabels rundet man deshalb meist auf die nächste metrische Größe auf. Prüfen Sie die Strombelastbarkeit des metrischen Kabels getrennt. Die Fläche allein bestimmt sie nicht, denn Isolierung, Verlegeart und Umgebungstemperatur ändern sie.

## Jede Größe umrechnen

An interactive calculator is on the web page: https://apps.schimpf.es/offline-wire-gauge-calculator/de/awg-to-mm2-chart/

## Grenzen dieser Tabelle

- Die Tabelle zeigt einen massiven Leiter. Feindrähtige Leiter haben denselben Nennquerschnitt, aber einen etwas größeren Außendurchmesser und einen etwas höheren Widerstand.
- Der Widerstand gilt bei 20 °C. Der Kupferwiderstand steigt um etwa 0,39 % je °C, ein Draht mit 75 °C hat also etwa 22 % mehr Widerstand.
- Spannungsfall-Berechnungen nach NEC verwenden die Widerstandswerte aus NFPA 70, Kapitel 9, Tabelle 8 (Ausgabe 2023). Diese gelten für eine andere Temperatur und für unbeschichtete Leiter und weichen leicht von den Werten oben ab. Diese Seite gibt keine NEC-Tabellen wieder.

## In der App nachschlagen

Der Kabelquerschnitt-Rechner hat diese Tabelle unter "Reference" eingebaut, für Kupfer und Aluminium, in mm² und in Ω je km und je 1000 ft. Sie funktioniert ohne Empfang. Die App ist auf Englisch. Dieselbe App ermittelt auch den Leiterquerschnitt nach NEC-Regeln für Strombelastbarkeit, Spannungsfall und Leitungsschutz. Jedes Ergebnis zeigt, welche Grenze den Querschnitt bestimmt hat und aus welcher NEC-Tabelle und Ausgabe es stammt. Die Ergebnisse sind Schätzwerte. Prüfen Sie sie anhand der örtlichen Vorschriften und der zuständigen Behörde.
