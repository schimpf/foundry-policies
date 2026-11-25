# 12-V-Kabelquerschnitt und Spannungsfall berechnen

> Kabelquerschnitt für 12 V und 24 V berechnen. Mit Spannungsfall-Formel, Rechenbeispiel und maximaler Leitungslänge je Querschnitt.

- Web: https://apps.schimpf.es/offline-wire-gauge-calculator/de/12v-wire-size-voltage-drop/
- App: Kabelquerschnitt-Rechner: NEC, https://apps.schimpf.es/offline-wire-gauge-calculator/de/index.md
Bei 12 V macht schon ein kleiner Spannungsverlust viel aus. 0,6 V Verlust sind bei 12 V 5 %, bei 240 V nur 0,25 %. Deshalb wird der Querschnitt bei 12-V- und 24-V-Leitungen (Wohnmobil, Camper, Boot, Solaranlage) meist zuerst nach dem Spannungsfall gewählt und danach auf Strombelastbarkeit geprüft. Diese Seite zeigt die Formel, ein Rechenbeispiel und eine Tabelle mit maximalen Längen.

## Die Spannungsfall-Formel für Gleichstrom

Der Strom fließt auf einem Leiter hin und auf dem anderen zurück. Deshalb zählt der Widerstand der doppelten einfachen Länge.

1. Spannungsfall in Volt: ΔU = 2 × L × I × R
2. Spannungsfall in Prozent: ΔU / Versorgungsspannung × 100
3. Zulässiger Spannungsfall in Volt: Ziel in % / 100 × Versorgungsspannung
4. Maximale einfache Länge: L max = zulässiger Spannungsfall / (2 × I × R)

L ist die einfache Länge in Metern, I der Strom in Ampere und R der Leiterwiderstand in Ohm pro Meter (der Wert aus der Tabelle in Ω/km geteilt durch 1000). Bei Gleichstrom ergibt Watt geteilt durch Volt den Strom in Ampere.

Ein gängiges Ziel für einen Abzweig ist 3 %. NFPA 70 (die NEC), Ausgabe 2023, nennt 3 % für einen Abzweigstromkreis und 5 % für Zuleitung und Abzweig zusammen, in Hinweisen (informational notes) zu Artikel 210 und 215. Diese Hinweise sind nur Empfehlungen. Sie können ein strengeres Ziel wählen, zum Beispiel für empfindliche Elektronik oder LED-Beleuchtung.

## Kupferwiderstand für die Beispiele

Die Werte gelten für massives Kupfer bei 20 °C. Sie sind aus der öffentlichen AWG-Durchmesserformel und dem spezifischen Widerstand von geglühtem Kupfer berechnet. Wie das geht, steht in der [AWG-mm²-Tabelle](awg-to-mm2-chart).

| AWG | mm² | Ω/km |
|---|---|---|
| 12 | 3,31 | 5,21 |
| 10 | 5,26 | 3,28 |
| 8 | 8,37 | 2,06 |
| 6 | 13,3 | 1,30 |
| 4 | 21,2 | 0,815 |

## Rechenbeispiel: 240 W Last, 5 m von der Batterie

Eine 12-V-Last nimmt 240 W auf. Die Leitung ist 5 m lang (einfach). Kupfer, Ziel 3 %.

1. Strom: 240 W / 12 V = 20 A.
2. Zulässiger Spannungsfall: 3 % × 12 V = 0,36 V.
3. Hin- und Rückweg: 2 × 5 m = 10 m. Mal Strom: 10 × 20 = 200 m·A.
4. Jeden Querschnitt prüfen:

| AWG | Spannungsfall (V) | Spannungsfall (%) | Innerhalb von 3 %? |
|---|---|---|---|
| 12 | 1,04 | 8,7 | Nein |
| 10 | 0,655 | 5,5 | Nein |
| 8 | 0,412 | 3,4 | Nein, knapp darüber |
| 6 | 0,259 | 2,2 | Ja |
| 4 | 0,163 | 1,4 | Ja |

5. Der kleinste Querschnitt, der besteht, ist 6 AWG (13,3 mm², nächste Normgröße 16 mm²). Spannungsfall bei 6 AWG: 200 × 0,001297 = 0,259 V, also 2,16 %.

8 AWG verliert 3,4 % und verfehlt das Ziel von 3 %. Prüfen Sie deshalb jeden Querschnitt, bevor Sie runden.

## Maximale einfache Länge bei 20 A, 12 V, 3 %

Hier gilt L max = 0,36 / (2 × 20 × R).

| AWG | Max. Länge (m) |
|---|---|
| 10 | 2,7 |
| 8 | 4,4 |
| 6 | 6,9 |
| 4 | 11,0 |

Bei 24 V verdoppelt sich der zulässige Spannungsfall in Volt. Dieselbe Last braucht nur den halben Strom, deshalb ist die maximale Länge bei gleichem Leiter viermal so groß.

## Strombelastbarkeit gilt weiterhin

Der Spannungsfall ist nur eine Grenze. Der Leiter muss den Strom auch tragen, und der Schutzschalter muss den Leiter schützen. Bei Dauerlast verlangt die NEC, den Stromkreis für 125 % der Last auszulegen (NFPA 70, Ausgabe 2023, 210.19(A)(1) und 215.2(A)(1)). Ein bestandener Spannungsfall-Test ersetzt die Prüfung der Strombelastbarkeit nicht. Der größere der beiden Querschnitte gilt.

## Wechselstrom

Bei Wechselstrom steht in der Formel die Impedanz statt des reinen Widerstands:

- Wirksame Ohm pro Meter: R × cos θ + X × sin θ. Dabei ist cos θ der Leistungsfaktor, R der Widerstand und X die Reaktanz.
- Einphasig: der Faktor 2 bleibt.
- Dreiphasig: der Faktor 2 wird zu √3 (1,732).

Die NEC führt R und X in Kapitel 9, Tabelle 9. Tabelle 8 enthält die Gleichstromwiderstände. Die Werte in den Tabellen oben stammen aus der öffentlichen Formel bei 20 °C. Sie weichen leicht von den NEC-Tabellen ab, und am Rand kann sich das Ergebnis um eine Größe unterscheiden.

## In der App rechnen

Der Kabelquerschnitt-Rechner (englischsprachige App) übernimmt diese Rechnung ohne Empfang. Geben Sie Ampere oder Watt und Volt, die Länge und Ihr Ziel ein. Die App prüft Spannungsfall, Strombelastbarkeit, die Regeln für den Schutzschalter und die Anschlussklasse und zeigt, welche Grenze den Querschnitt bestimmt. Sie nutzt NEC Kapitel 9 Tabelle 8 für Gleichstrom und Tabelle 9 für Wechselstrom und nennt Tabelle und Ausgabe in jedem Ergebnis. Dazu gibt es zwei Rückwärts-Modi: maximale Länge für einen gewählten Leiter und maximale Last für einen gewählten Leiter und eine Länge. Die DC-Voreinstellungen decken 12 V und 24 V ab, und 18 AWG und 16 AWG gibt es für DC. Länge wählen Sie in Metern oder Fuß.

Die Ergebnisse sind Schätzwerte. Prüfen Sie sie anhand der örtlichen Vorschriften und der zuständigen Behörde.
