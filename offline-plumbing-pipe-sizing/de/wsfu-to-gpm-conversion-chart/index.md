# WSFU in GPM umrechnen, Tabelle nach Hunter-Kurve

> WSFU in GPM und l/min umrechnen mit der Hunter-Kurve. Werte für Spülkasten und Druckspüler, dazu ein Rechenbeispiel.

- Web: https://apps.schimpf.es/offline-plumbing-pipe-sizing/de/wsfu-to-gpm-conversion-chart/
- App: Rohrdimensionierung IPC & UPC, https://apps.schimpf.es/offline-plumbing-pipe-sizing/de/index.md
Anschlusswerte (WSFU, water supply fixture units) geben an, wie stark ein Entnahmegegenstand eine Wasserleitung belastet. Für die Rohrbemessung brauchen Sie den Durchfluss in Gallonen pro Minute (GPM). Die Hunter-Kurve verbindet beide Größen. Diese Seite zeigt eine Umrechnungstabelle, erklärt die beiden Kurven und rechnet ein Beispiel von Hand durch.

Umrechnung: 1 GPM = 3,785 l/min. In Deutschland ist der Durchfluss in l/s oder l/min üblich, hier stehen beide Angaben.

## Was die Hunter-Kurve ist

Nicht jeder Entnahmegegenstand läuft gleichzeitig. Roy B. Hunter schätzte mit Wahrscheinlichkeitsrechnung den Spitzendurchfluss, den eine Gruppe von Entnahmegegenständen tatsächlich zieht. Seine Arbeit *Methods of Estimating Loads in Plumbing Systems* (National Bureau of Standards, Building Materials and Structures Report BMS 65, 1940) ist gemeinfrei und bis heute die Grundlage der Bedarfstabellen in den US-Installationsnormen.

Es gibt zwei Kurven:

- Spülkasten, für Anlagen, in denen die WCs einen Spülkasten haben. Sie ergibt einen niedrigeren Spitzendurchfluss.
- Druckspüler (Flushometer), für Anlagen, in denen die WCs Druckspüler haben. Sie ergibt einen höheren Spitzendurchfluss, weil ein Druckspüler in kurzer Zeit viel Wasser zieht.

Wählen Sie die Kurve nach der WC-Art. Ein Auftrag mit Druckspülern nutzt die Druckspüler-Kurve für den ganzen Abschnitt.

## Tabelle WSFU in GPM

Ausgewählte Punkte der Kurven. Werte dazwischen ergeben sich durch lineare Interpolation. Die Angaben in Klammern sind l/min.

| WSFU gesamt | Spülkasten, GPM (l/min) | Druckspüler, GPM (l/min) |
|---|---|---|
| 5 | 9,4 (35,6) | 15,0 (56,8) |
| 10 | 14,6 (55,3) | 27,0 (102) |
| 20 | 19,6 (74,2) | 35,0 (132) |
| 30 | 23,3 (88,2) | 42,0 (159) |
| 40 | 26,3 (99,6) | 46,0 (174) |
| 50 | 29,1 (110) | 50,0 (189) |
| 100 | 43,5 (165) | 67,5 (256) |
| 200 | 65,0 (246) | 90,0 (341) |
| 300 | 85,0 (322) | 108,0 (409) |
| 500 | 124,0 (469) | 143,0 (541) |
| 1.000 | 208,0 (787) | 208,0 (787) |

Hinweise zu den Bereichen:

- Die Spülkasten-Kurve reicht von 1 bis 5.000 WSFU. Bei 1 WSFU sind es 3,0 GPM, bei 2 WSFU 5,0 GPM.
- Die Druckspüler-Kurve reicht von 5 bis 5.000 WSFU.
- Ab 1.000 WSFU fallen die beiden Kurven zusammen. Große Anlagen haben so viele Entnahmegegenstände, dass die WC-Art den Spitzendurchfluss nicht mehr ändert.

## So rechnen Sie um

1. Addieren Sie die WSFU aller Entnahmegegenstände, die das Rohr versorgt, mit den Werten aus Ihrer geltenden Norm.
2. Wählen Sie die Spülkasten- oder die Druckspüler-Kurve.
3. Suchen Sie die beiden Tabellenpunkte links und rechts Ihrer Summe.
4. Interpolieren Sie zwischen ihnen.

Die Interpolation lautet:

**GPM = GPM₁ + (WSFU − WSFU₁) / (WSFU₂ − WSFU₁) × (GPM₂ − GPM₁)**

## Rechenbeispiel

Eine Badgruppe an einer Anlage mit Spülkasten hat zusammen 22 WSFU.

1. Die Tabellenpunkte auf beiden Seiten sind 20 WSFU (19,6 GPM) und 25 WSFU (21,5 GPM).
2. Die Position dazwischen ist (22 − 20) / (25 − 20) = 0,4.
3. GPM = 19,6 + 0,4 × (21,5 − 19,6) = 19,6 + 0,76 = 20,36, gerundet 20,4 GPM (77,2 l/min).

Dieselben 22 WSFU an einer Anlage mit Druckspülern:

1. Punkte: 20 WSFU (35,0 GPM) und 25 WSFU (38,0 GPM).
2. GPM = 35,0 + 0,4 × (38,0 − 35,0) = 36,2 GPM (137 l/min).

Die Anlage mit Druckspülern braucht für dieselben Anschlusswerte fast 16 GPM (rund 60 l/min) mehr.

## Was Sie mit dem Durchfluss tun

Der Durchfluss allein ergibt noch keine Rohrgröße. Als Nächstes vergleichen Sie die Geschwindigkeit je Rohrgröße mit einer Grenze und prüfen den Druckverlust. Die Formeln stehen auf der Hazen-Williams-Seite dieser Website.

Beispiel: 20,4 GPM in Kupfer Typ L (Innendurchmesser 1,025 Zoll bei 1", also 26,0 mm) ergeben eine Geschwindigkeit von 0,4085 × 20,4 / 1,025² = 7,9 fps (2,4 m/s). Das liegt knapp innerhalb einer Kaltwassergrenze von 8 fps (2,44 m/s), also reicht 1". Bei 36,2 GPM würde dasselbe Rohr mit 14,1 fps (4,3 m/s) strömen, und Sie bräuchten 1-1/2" (6,5 fps, 2,0 m/s).

## Grenzen des Verfahrens

- Die Hunter-Kurve liefert eine Spitzenschätzung für übliche Mischungen von Entnahmegegenständen. Dauerlasten wie Bewässerung oder Prozesswasser kommen gesondert dazu.
- Moderne Spararmaturen ziehen oft weniger, als die Kurve vorhersagt. Die Normen nutzen die Kurve weiter, richten Sie sich also nach der geltenden Norm.
- Ihre geltende Norm bestimmt, welche WSFU-Werte und welche Ausgabe gelten. Die IPC (Ausgabe 2024) behandelt den Bedarf in Anhang E, Abschnitt E103.3. Die UPC (Ausgabe 2024) behandelt ihn in Anhang A, Abschnitt A 103.0.
- Gedruckte Normtabellen können leicht von den so berechneten Kurvenwerten abweichen.
- In Deutschland wird der Spitzendurchfluss nach DIN 1988-300 aus Berechnungsdurchflüssen ermittelt, nicht aus WSFU. Die Tabelle gilt für US-Normen und ersetzt dieses Verfahren nicht.

## Umrechnen und bemessen in der App

Die Android-App Offline Plumbing Pipe Sizing nimmt Ihnen diese Umrechnung ab. Sie geben die WSFU-Summe ein und stellen einmal Spülkasten oder Druckspüler ein, dann rechnet die App mit der Hunter-Kurve in GPM um. Danach zeigt sie die empfohlene Rohrgröße, die Geschwindigkeit und den Druckverlust in psi pro 100 ft für jede Größe von 1/2" bis 4". Sie funktioniert ohne Verbindung und nennt den Abschnitt der IPC oder UPC für die gewählte Ausgabe. Die App ist auf Englisch und rechnet nur in US-Einheiten.

## Quellen

- Hunter, R. B., *Methods of Estimating Loads in Plumbing Systems*, National Bureau of Standards, Building Materials and Structures Report BMS 65, 1940.
- International Plumbing Code (ICC), 2024 edition, Appendix E.
- Uniform Plumbing Code (IAPMO), 2024 edition, Appendix A.
