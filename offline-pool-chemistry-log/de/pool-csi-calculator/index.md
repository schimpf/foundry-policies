# Pool-CSI-Rechner: Sättigungsindex erklärt

> Berechne den Calcit-Sättigungsindex (CSI) deines Poolwassers mit Formel und Rechenbeispiel und erfahre, was du bei einem Wert außerhalb ändern musst.

- Web: https://apps.schimpf.es/offline-pool-chemistry-log/de/pool-csi-calculator/
- App: Pool Chem Log: Wassertests, https://apps.schimpf.es/offline-pool-chemistry-log/de/index.md
Der Calcit-Sättigungsindex (CSI) zeigt, ob dein Poolwasser eher Putz und Metall angreift oder Kalk absetzt. Ein CSI nahe null bedeutet ausgewogenes Wasser. Diese Seite bietet dir einen Rechner, die Formel und ein Rechenbeispiel.

## CSI-Rechner

An interactive calculator is on the web page: https://apps.schimpf.es/offline-pool-chemistry-log/de/pool-csi-calculator/

## So liest du das Ergebnis

- **Unter -0,3:** korrosiv. Das Wasser kann Putz anätzen, Fugen beschädigen und Metallteile angreifen.
- **-0,3 bis +0,3:** ausgewogen. Diesen Bereich nutzt Pool Chem Log als Ziel.
- **Über +0,3:** kalkabscheidend. Kalk kann sich an Fliesen, Oberflächen sowie in der Salzzelle oder der Heizung ablagern.

Der Bereich von -0,3 bis +0,3 ist ein praktisches Ziel. Pools mit Putzoberfläche profitieren am meisten davon, in ihm zu bleiben.

## Was in den CSI eingeht

Der CSI nutzt diese Testergebnisse:

- pH
- Gesamtalkalinität (TA) in ppm (in Deutschland oft als Säurekapazität in mmol/l angegeben: 1 mmol/l entspricht etwa 50 ppm)
- Calciumhärte (CH) in ppm (zeigt dein Test °dH, rechne um: 1 °dH entspricht etwa 17,8 ppm)
- Cyanursäure (CYA) in ppm
- Borate in ppm (optional)
- Salz in ppm
- Wassertemperatur in °C

Warmes Wasser scheidet eher Kalk ab, deshalb zählt die Temperatur. Salz wirkt über die Ionenstärke nur wenig. Wenn du deinen Salzgehalt nicht kennst, rechnet der Rechner mit 1.000 ppm. Das ist typisch für Füllwasser plus Chlor-Nebenprodukte. Lässt du CYA oder Borate leer, zählen sie als 0. 1 ppm entspricht 1 mg/l.

## Die Formel

Die Formel ist die von Trouble Free Pool (TFP) und Pool Math, die dem Chemiker "chem geek" zugeschrieben wird.

CSI = pH - 6,9395 + log10(CH) + log10(Carbonat-Alkalinität) - 2,56 × sqrt(I) / (1 + 1,65 × sqrt(I)) - 1412,5 / T

Dabei gilt:

- **Carbonat-Alkalinität** = TA - 0,38772 × CYA / (1 + 10^(6,83 - pH)) - 4,63 × Borate / (1 + 10^(9,11 - pH)). CYA und Borate zählen im Testset zur TA, helfen aber nicht dem Carbonat-Gleichgewicht, deshalb werden sie abgezogen.
- **I (Ionenstärke)** = (1,5 × CH + TA) / 50045 + Salz / 58440.
- **T** ist die Wassertemperatur in Kelvin: Grad Celsius + 273,15.

Ist CH gleich 0 oder die Carbonat-Alkalinität 0 oder kleiner, lässt sich der CSI nicht berechnen.

## Rechenbeispiel

Ein Pool mit Putzoberfläche hat diese Testwerte:

- pH 7,5
- TA 70 ppm
- CH 350 ppm
- CYA 40 ppm
- Borate 0
- Salz 1.000 ppm (angenommen)
- Wasser 27 °C, das sind 300,15 K

Schritt für Schritt:

1. Carbonat-Alkalinität: 10^(6,83 - 7,5) = 0,2138, also CYA-Anteil = 0,38772 × 40 / 1,2138 = 12,78. Carbonat-Alkalinität = 70 - 12,78 = 57,22.
2. Ionenstärke: (1,5 × 350 + 70) / 50045 + 1000 / 58440 = 0,01189 + 0,01711 = 0,02900. Die Wurzel daraus ist 0,1703.
3. Ionen-Term: 2,56 × 0,1703 / (1 + 1,65 × 0,1703) = 0,4360 / 1,2810 = 0,3403.
4. Temperatur-Term: 1412,5 / 300,15 = 4,7060.
5. Logarithmen: log10(350) = 2,5441 und log10(57,22) = 1,7576.
6. Zusammenzählen: 7,5 - 6,9395 + 2,5441 + 1,7576 - 0,3403 - 4,7060 = -0,18.

Der CSI liegt bei etwa -0,18. Das ist im ausgewogenen Bereich, etwas zur weichen Seite.

## Was du ändern kannst, wenn der CSI abweicht

Ist der CSI zu niedrig (korrosiv), erhöhe einen dieser Werte:

- **Calciumhärte:** der größte Hebel bei Pools mit Putzoberfläche. Calciumchlorid erhöht sie, aber langsam, deshalb gib es in Schritten zu.
- **pH:** Eine Erhöhung des pH um 0,1 erhöht den CSI um etwa 0,1.
- **Gesamtalkalinität:** Natron (Natriumhydrogencarbonat) erhöht sie.

Ist der CSI zu hoch (kalkabscheidend), senke den pH mit Säure oder senke die TA. Calcium zu senken heißt Wasser auszutauschen, denn kein Produkt entfernt es.

Die Calciumziele in Pool Chem Log hängen von der Oberfläche ab:

| Oberfläche | CH-Bereich (ppm) |
|---|---|
| Putz oder Kiesel | 250 bis 650 |
| Folie oder GFK | 50 bis 350 |
| Acryl | 150 bis 250 (üblicher Bereich) |

Die Bereiche für Putz, Kiesel, Folie und GFK folgen den TFP-Hinweisen. Der Bereich für Acryl ist ein in der Branche üblicher Bereich.

## Borate und Salz

Borate sind optional. Manche Besitzer halten 30 bis 50 ppm als pH-Puffer. Wenn du sie nutzt, nimm sie in die Berechnung auf, denn Borate erhöhen den TA-Messwert, ohne das Gleichgewicht zu verbessern. Salzwasser-Pools sollten ihren tatsächlichen Salzgehalt eingeben.

## Grenzen

Der CSI ist ein Modell und hängt von genauen Tests ab, besonders bei TA, CH und pH. Ein kleiner Messfehler kann den CSI um 0,1 oder mehr verschieben. Teste erneut, bevor du etwas Großes änderst, mische niemals Chemikalien, trage Schutzausrüstung und folge dem Etikett des Produkts.

## CSI im Verlauf verfolgen

Pool Chem Log ist eine Android-App, die ohne Internet funktioniert. Sie berechnet den CSI bei jedem Test, den du einträgst, mit Boraten und Salz, und nimmt dafür die Temperatur aus dem letzten Test. Sie zeigt außerdem deine Zielwerte nach Oberfläche, berechnet Dosierungen für Calcium, Alkalinität und pH und führt einen Verlauf aller deiner Tests. Die Formel in der App ist dieselbe wie auf dieser Seite.
