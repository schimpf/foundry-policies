# Hazen-Williams-Formel für den Druckverlust im Rohr

> Hazen-Williams-Formel für den Druckverlust in Wasserleitungen, mit C-Werten für Kupfer und PEX, Umrechnung in mbar/m und einem Rechenbeispiel.

- Web: https://apps.schimpf.es/offline-plumbing-pipe-sizing/de/hazen-williams-friction-loss-formula/
- App: Rohrdimensionierung IPC & UPC, https://apps.schimpf.es/offline-plumbing-pipe-sizing/de/index.md
Hazen-Williams ist das gängige Verfahren, um den Druckverlust in Wasserleitungen abzuschätzen. Es ist einfach, rechnet in US-Einheiten und ist für die Bemessung von Kalt- und Warmwasserleitungen genau genug. Diese Seite zeigt die Formel, die C-Werte für Kupfer und Kunststoff und ein Rechenbeispiel, das Sie mit einem Taschenrechner nachvollziehen können.

Umrechnung: 1 GPM = 3,785 l/min, 1 fps = 0,3048 m/s, 1 ft = 0,3048 m, 1 Zoll = 25,4 mm, 1 psi = 68,95 mbar, 1 psi pro 100 ft = 2,262 mbar/m.

## Die Formel

Für Wasser in einem vollen Rohr beträgt der Druckverlust in psi pro 100 Fuß Rohrlänge:

**psi pro 100 ft = 100 × 4,52 × Q^1,852 / (C^1,852 × d^4,8704)**

Dabei gilt:

- Q ist der Durchfluss in Gallonen pro Minute (GPM).
- C ist der Rauheitsbeiwert nach Hazen-Williams. Ein höheres C bedeutet ein glatteres Rohr.
- d ist der tatsächliche Innendurchmesser des Rohrs in Zoll. Die Nennweite gehört nicht in die Formel.

Die Formel geht auf die Arbeit von Williams und Hazen zurück (*Hydraulic Tables*, 1905). Die Form oben ist die in den USA übliche Version mit US-Einheiten, wie sie in Nachschlagewerken für Sanitär und Brandschutz steht.

Für den Verlust über eine Leitung skalieren Sie mit der Länge:

**Verlust in psi = psi pro 100 ft × Länge in ft / 100**

Das gilt nur für gerades Rohr. Formstücke, Armaturen und Wasserzähler verursachen zusätzlichen Verlust, den die Formel nicht enthält.

## Geschwindigkeit

Die Geschwindigkeit ist so wichtig wie die Reibung. Schnelles Wasser verursacht Geräusche und Erosion, deshalb beginnt die Bemessung meist mit einer Geschwindigkeitsgrenze.

**Geschwindigkeit in fps = 0,4085 × Q / d²**

Q ist in GPM angegeben und d ist der Innendurchmesser in Zoll.

## Zu verwendende C-Werte

Auslegungswerte, niedriger als die Bestwerte für neue Rohre:

| Material | C |
|---|---|
| Kupfer (Typ K, L, M) | 130 |
| PEX, PE-RT, CPVC, PEX-AL-PEX | 150 |

## Den Innendurchmesser verwenden

Die Nennweite ist nur ein Name. Kupferrohr wird nach Nenndurchmesser bezeichnet, und der echte Innendurchmesser ändert sich mit der Wandstärke. Diese Innendurchmesser gelten auf dieser Seite, nach ASTM B88 (Kupfer Typ L) und ASTM F876 (PEX, SDR 9). Sie gelten für US-Rohre. Europäisches Kupferrohr nach EN 1057 hat andere Innendurchmesser.

| Nennweite | Kupfer L, Innendurchm. in Zoll (mm) | PEX SDR 9, Innendurchm. in Zoll (mm) |
|---|---|---|
| 1/2" (DN 15) | 0,545 (13,8) | 0,475 (12,1) |
| 3/4" (DN 20) | 0,785 (19,9) | 0,671 (17,0) |
| 1" (DN 25) | 1,025 (26,0) | 0,862 (21,9) |
| 1-1/4" (DN 32) | 1,265 (32,1) | 1,054 (26,8) |
| 1-1/2" (DN 40) | 1,505 (38,2) | 1,244 (31,6) |
| 2" (DN 50) | 1,985 (50,4) | 1,629 (41,4) |

Die DN-Werte sind ungefähre Entsprechungen. Weil die Reibung von d hoch 4,87 abhängt, wirkt sich eine kleine Änderung des Innendurchmessers stark aus. Eine PEX-Leitung ist für denselben Durchfluss oft eine Größe größer als Kupfer.

## Rechenbeispiel

Ein Strang versorgt 10 Anschlusswerte (WSFU, water supply fixture units) mit Spülkasten. Nach der Hunter-Kurve sind 10 WSFU gleich 14,6 GPM (55,3 l/min). Das Rohr ist Kupfer Typ L (C = 130) und die Geschwindigkeitsgrenze für Kaltwasser beträgt 8 fps (2,44 m/s). Die Leitung ist 60 ft (18,3 m) lang.

Schritt 1, jede Größe prüfen. Berechnen Sie die Geschwindigkeit mit 0,4085 × 14,6 / d², das sind 5,964 / d²:

| Größe | Innendurchm. in Zoll | Geschwindigkeit in fps (m/s) | Druckverlust in psi/100 ft (mbar/m) | Innerhalb 8 fps? |
|---|---|---|---|---|
| 1/2" | 0,545 | 20,1 (6,1) | 152 (344) | Nein |
| 3/4" | 0,785 | 9,68 (2,95) | 25,6 (57,9) | Nein |
| 1" | 1,025 | 5,68 (1,73) | 6,99 (15,8) | Ja |

Schritt 2, die kleinste Größe innerhalb der Grenze wählen. Das ist 1".

Schritt 3, den Druckverlust für 1" von Hand berechnen.

1. 14,6^1,852 = 143,3
2. 130^1,852 = 8.223
3. 1,025^4,8704 = 1,128
4. psi pro 100 ft = 100 × 4,52 × 143,3 / (8.223 × 1,128) = 64.785 / 9.274 = 6,99

Schritt 4, auf 60 ft hochrechnen. 6,99 × 60 / 100 = 4,19 psi Verlust über die gerade Leitung (289 mbar, also etwa 0,29 bar).

Derselbe Durchfluss in 3/4" Kupfer würde 25,6 psi pro 100 ft verlieren und mit fast 10 fps (knapp 3 m/s) strömen. Deshalb kommt die Geschwindigkeitsprüfung zuerst.

## Ausprobieren

An interactive calculator is on the web page: https://apps.schimpf.es/offline-plumbing-pipe-sizing/de/hazen-williams-friction-loss-formula/

Der Rechner nutzt die Formeln und Innendurchmesser von oben und arbeitet in GPM, Zoll, Fuß und psi. Die Ergebnisse sind berechnete Werte und können leicht von gedruckten Tabellen abweichen.

## Was diese Seite nicht abdeckt

- Formstücke und Armaturen. Rechnen Sie deren Verlust gesondert dazu.
- Höhenunterschiede und Netzdruck.
- Wasser, das nicht normales Trinkwasser bei üblichen Temperaturen ist.

Prüfen Sie für Bemessungsregeln und Mindestgrößen die geltende Installationsnorm und die zuständige Behörde. Die IPC (Ausgabe 2024) behandelt die Rohrbemessung in Abschnitt 604.3 und Anhang E, die UPC (Ausgabe 2024) in Abschnitt 610.1 und Anhang A. In Deutschland richtet sich die Bemessung nach DIN 1988-300, die den Druckverlust über das Rohrreibungsgefälle in mbar/m berechnet. Hazen-Williams mit US-Rohren ersetzt diese Berechnung nicht.

## Vor Ort rechnen

Die Android-App Offline Plumbing Pipe Sizing führt diese Berechnung für jede Größe von 1/2" bis 4" auf einmal aus. Sie geben WSFU oder GPM ein und wählen ein Material. Die App zeigt die empfohlene Größe, die Geschwindigkeit und die psi pro 100 ft in einer Tabelle. Mit einer Abschnittslänge ergänzt sie den Gesamtverlust der geraden Leitung. Sie funktioniert ohne Verbindung und nennt den Abschnitt der IPC oder UPC für die gewählte Ausgabe (2024 oder 2021). Kupfer L und PEX sind ab dem ersten Start nutzbar. Die App ist auf Englisch und rechnet nur in US-Einheiten.

## Quellen

- Williams, G. S. and Hazen, A., *Hydraulic Tables*, 1905.
- ASTM B88, Standard Specification for Seamless Copper Water Tube (inside diameters, Type L).
- ASTM F876, Standard Specification for Crosslinked Polyethylene (PEX) Tubing (SDR 9 inside diameters).
- International Plumbing Code (ICC), 2024 edition, section 604.3 and Appendix E.
- Uniform Plumbing Code (IAPMO), 2024 edition, section 610.1 and Appendix A.
