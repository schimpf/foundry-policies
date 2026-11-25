# Kupfer und PEX Rohrgrößen-Tabelle nach Durchfluss (GPM)

> Maximaler Durchfluss in GPM und l/min für Kupfer Typ L und PEX von 1/2 bis 4 Zoll bei 5 und 8 fps, mit Innendurchmessern und Rechenbeispiel.

- Web: https://apps.schimpf.es/offline-plumbing-pipe-sizing/de/copper-and-pex-pipe-size-chart-gpm/
- App: Rohrdimensionierung IPC & UPC, https://apps.schimpf.es/offline-plumbing-pipe-sizing/de/index.md
Ein Kupferrohr Typ L mit 3/4" führt bei 8 fps bis zu 12,07 GPM (45,7 l/min) und bei 5 fps bis zu 7,54 GPM (28,5 l/min). Der Höchstwert hängt von der Geschwindigkeit ab, die Sie zulassen, und vom tatsächlichen Innendurchmesser des Rohrs. Diese Seite enthält eine Tabelle des maximalen Durchflusses je Rohrgröße für Kupfer Typ L und PEX, zeigt, wie die Zahlen entstehen, und bemisst eine Leitung für einen vorgegebenen Durchfluss.

Umrechnung: 1 GPM = 3,785 l/min, 1 fps = 0,3048 m/s, 1 Zoll = 25,4 mm.

## Warum die Geschwindigkeit die Größe bestimmt

Bei der Bemessung von Trinkwasserleitungen wählt man meist das kleinste Rohr, das unter einer Geschwindigkeitsgrenze bleibt. Schnelles Wasser macht Geräusche und greift das Rohr an, besonders in Warmwasserleitungen. Zwei Grenzen sind verbreitet:

- 8 fps (2,44 m/s) für Kaltwasser.
- 5 fps (1,52 m/s) für Warmwasser in Kupfer.

Die IPC nennt für diese Materialien keine Geschwindigkeitsgrenze. Die Werte stammen aus Angaben von Herstellern und der Copper Development Association (*Copper Tube Handbook*). Die UPC (Ausgaben 2024 und 2021, Anhang A, Abschnitt A 105.1) nennt 8 fps für Kaltwasser. Welche Grenze gilt, entscheidet die örtliche Behörde. Klären Sie das, bevor Sie sich auf einen Wert verlassen.

## Die Formel hinter der Tabelle

Stellen Sie die Geschwindigkeitsgleichung um, um den Durchfluss zu erhalten, den ein Rohr bei einer bestimmten Geschwindigkeit führt:

**GPM = Geschwindigkeit in fps × d² / 0,4085**

Dabei ist d der Innendurchmesser in Zoll. Bei 8 fps gilt GPM = 19,58 × d². Bei 5 fps gilt GPM = 12,24 × d².

## Innendurchmesser

Die Innendurchmesser stammen aus ASTM B88 (Kupfer Typ L) und ASTM F876 (PEX, SDR 9). Die Nennweite ist nur eine Bezeichnung. Die Werte gelten für US-Rohre. Europäisches Kupferrohr nach EN 1057 und PEX-Rohre mit Maßen in mm haben andere Innendurchmesser.

## Maximaler Durchfluss, Kupfer Typ L

Die Angaben in Klammern sind l/min. Die DN-Werte sind ungefähre Entsprechungen.

| Nennweite | Innendurchm. in Zoll (mm) | Max. GPM (l/min) bei 8 fps (kalt) | Max. GPM (l/min) bei 5 fps (warm) |
|---|---|---|---|
| 1/2" (DN 15) | 0,545 (13,8) | 5,82 (22,0) | 3,64 (13,8) |
| 3/4" (DN 20) | 0,785 (19,9) | 12,07 (45,7) | 7,54 (28,5) |
| 1" (DN 25) | 1,025 (26,0) | 20,58 (77,9) | 12,86 (48,7) |
| 1-1/4" (DN 32) | 1,265 (32,1) | 31,34 (119) | 19,59 (74,2) |
| 1-1/2" (DN 40) | 1,505 (38,2) | 44,36 (168) | 27,72 (105) |
| 2" (DN 50) | 1,985 (50,4) | 77,17 (292) | 48,23 (183) |
| 2-1/2" (DN 65) | 2,465 (62,6) | 119,0 (450) | 74,37 (282) |
| 3" (DN 80) | 2,945 (74,8) | 169,9 (643) | 106,2 (402) |
| 4" (DN 100) | 3,905 (99,2) | 298,6 (1130) | 186,6 (706) |

## Maximaler Durchfluss, PEX (SDR 9)

Für PEX gilt in den hier verwendeten Herstellerangaben keine 5-fps-Grenze für Warmwasser. Eine Spalte bei 8 fps deckt daher beide Fälle ab.

| Nennweite | Innendurchm. in Zoll (mm) | Max. GPM (l/min) bei 8 fps |
|---|---|---|
| 1/2" (DN 15) | 0,475 (12,1) | 4,42 (16,7) |
| 3/4" (DN 20) | 0,671 (17,0) | 8,82 (33,4) |
| 1" (DN 25) | 0,862 (21,9) | 14,55 (55,1) |
| 1-1/4" (DN 32) | 1,054 (26,8) | 21,76 (82,4) |
| 1-1/2" (DN 40) | 1,244 (31,6) | 30,31 (115) |
| 2" (DN 50) | 1,629 (41,4) | 51,97 (197) |
| 2-1/2" (DN 65) | 2,011 (51,1) | 79,20 (300) |
| 3" (DN 80) | 2,400 (61,0) | 112,8 (427) |
| 4" (DN 100) | 3,162 (80,3) | 195,8 (741) |

Vergleichen Sie beide Tabellen. Bei gleicher Nennweite führt PEX weniger, weil die Wand dicker und der Innendurchmesser kleiner ist. Ein 1"-PEX-Rohr führt bei 8 fps etwa 14,5 GPM (55 l/min), ein 1"-Kupferrohr Typ L etwa 20,6 GPM (78 l/min).

## So nutzen Sie die Tabelle

1. Bestimmen Sie Ihren Auslegungsdurchfluss in GPM (1 l/min = 0,2642 GPM). Wenn Sie Anschlusswerte (WSFU) haben, rechnen Sie diese mit der Hunter-Kurve um (siehe die Seite WSFU in GPM auf dieser Website).
2. Wählen Sie das Material und die Geschwindigkeitsgrenze.
3. Gehen Sie in der Spalte nach unten bis zur ersten Größe, deren maximaler Durchfluss Ihrem Durchfluss entspricht oder darüber liegt.

## Rechenbeispiel

Eine Warmwasserleitung aus Kupfer Typ L muss 14,6 GPM (55,3 l/min, 0,92 l/s) führen. Es gilt die Warmwassergrenze von 5 fps.

1. 3/4" schafft höchstens 7,54 GPM und ist zu klein.
2. 1" schafft höchstens 12,86 GPM und ist noch immer zu klein.
3. 1-1/4" schafft höchstens 19,59 GPM. Das ist die erste Größe, die passt.

Prüfen Sie die Geschwindigkeit: 0,4085 × 14,6 / 1,265² = 3,7 fps (1,14 m/s). Derselbe Durchfluss in einer Kaltwasserleitung mit 8 fps passt in 1" (5,7 fps, 1,73 m/s).

## Auch den Druckverlust prüfen

Die Geschwindigkeit ist nur ein Teil der Prüfung, denn lange Leitungen verlieren Druck. Der Druckverlust nach Hazen-Williams für das Kaltwasserbeispiel oben (14,6 GPM, 1" Kupfer Typ L, C = 130) beträgt etwa 6,99 psi pro 100 ft (15,8 mbar/m). Über eine Leitung von 60 ft (18,3 m) sind das etwa 4,2 psi (0,29 bar). Die Seite zu Hazen-Williams auf dieser Website zeigt die vollständige Rechnung.

## Grenzen dieser Tabelle

- Die Werte sind berechnet und können leicht von gedruckten Tabellen abweichen.
- Die Mindestgrößen der Norm gelten weiterhin. Die IPC 2024 verlangt zum Beispiel mindestens 3/4" für einen Hausanschluss (Abschnitt 603.1), die UPC 2024 mindestens 3/4" für die Gebäudezuleitung (Abschnitt 610.8). Ein Tabellenwert von 1/2" setzt das nicht außer Kraft.
- Formstücke, Wasserzähler, Höhenunterschiede und Netzdruck sind nicht Teil dieser Tabelle.
- In Deutschland richtet sich die Bemessung nach DIN 1988-300. Diese Tabelle rechnet mit US-Rohren und US-Geschwindigkeitsgrenzen und ersetzt diese Berechnung nicht.

## Die App statt der Tabelle nutzen

Die Android-App Offline Plumbing Pipe Sizing erstellt diese Tabelle für Ihren genauen Durchfluss. Sie geben GPM oder WSFU ein, wählen IPC oder UPC, die Ausgabe 2024 oder 2021 und ein Material. Die App markiert die kleinste Größe innerhalb der Geschwindigkeitsgrenze und listet Geschwindigkeit und psi pro 100 ft für jede Größe von 1/2" bis 4" auf. Sie können die Geschwindigkeitsgrenze zwischen 1 und 20 fps ändern und auf den Standard zurücksetzen. Die App funktioniert ohne Verbindung. Kupfer L und PEX sind ab dem ersten Start verfügbar. Kupfer K und M, CPVC, PEX-AL-PEX und PE-RT sowie gespeicherte Aufträge gehören zum einmaligen Pro-Kauf. Die App ist auf Englisch und rechnet nur in US-Einheiten.

## Quellen

- ASTM B88, Standard Specification for Seamless Copper Water Tube (inside diameters, Type L).
- ASTM F876, Standard Specification for Crosslinked Polyethylene (PEX) Tubing (SDR 9 inside diameters).
- Copper Development Association, *Copper Tube Handbook* (velocity guidance for copper).
- International Plumbing Code (ICC), 2024 edition, section 603.1.
- Uniform Plumbing Code (IAPMO), 2024 edition, sections 610.8 and Appendix A, A 105.1.
