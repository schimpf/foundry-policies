# Vorgabezeit berechnen, Formel mit Rechenbeispiel

> So berechnest du Normalzeit und Vorgabezeit aus Stoppuhrwerten, Leistungsgrad und Zuschlag. Mit durchgerechnetem Beispiel und kleinem Rechner.

- Web: https://apps.schimpf.es/time-study-stopwatch/de/standard-time-formula-example/
- App: Zeitstudie Stoppuhr, https://apps.schimpf.es/time-study-stopwatch/de/index.md
Die Vorgabezeit ist die Zeit, die eine eingearbeitete Person für eine Tätigkeit in normalem Tempo braucht, plus Zeit für Erholung und unvermeidbare Störungen. Sie ist die Zahl hinter Zeitvorgaben, Taktabstimmung und Kapazitätsplanung. Diese Seite zeigt die Formel, ein durchgerechnetes Beispiel mit echten Zahlen und einen Rechner, den du sofort nutzen kannst.

## Die Formel

Die Vorgabezeit entsteht in zwei Schritten.

1. Normalzeit = gemessene Zeit × Leistungsgrad ÷ 100
2. Vorgabezeit = Normalzeit × (1 + Zuschlag ÷ 100)

Dabei gilt:

- Die gemessene Zeit ist der Wert, den die Stoppuhr für einen Ablaufabschnitt anzeigt.
- Der Leistungsgrad ist deine Einschätzung des Arbeitstempos. 100 % bedeutet normales Tempo. Über 100 % ist schneller als normal, unter 100 % langsamer.
- Der Zuschlag ist die zusätzliche Zeit für persönliche Bedürfnisse, Erholung und Störungen (englisch PF&D), als Prozentwert der Normalzeit.

Die Methode folgt den klassischen Werken der Arbeitsmessung, zum Beispiel Niebel und Freivalds, *Methods, Standards, and Work Design* (McGraw-Hill, 12. Auflage, 2009), und International Labour Office, *Introduction to Work Study* (4. Auflage, 1992). In Deutschland ist sie als Zeitaufnahme nach REFA bekannt, wo die Normalzeit Grundzeit heißt.

### Regeln in der App und auf dieser Seite

- Die Normalzeit wird pro Ablaufabschnitt berechnet. Jede Beobachtung wird mit ihrem Leistungsgrad multipliziert, danach wird der Mittelwert gebildet.
- Die Normalzeiten aller Ablaufabschnitte werden zur normalen Zykluszeit addiert.
- Der Zuschlag ist ein Aufschlag auf die Normalzeit. Ein Zuschlag von 15 % multipliziert die Normalzeit mit 1,15.
- Der Zuschlag ist von 0 bis 100 % zulässig.
- Der Leistungsgrad ist von 50 bis 200 % zulässig.

Manche Quellen beziehen den Zuschlag auf die gesamte Arbeitszeit. Dann gilt Vorgabezeit = Normalzeit ÷ (1 − Zuschlag ÷ 100), was andere Ergebnisse liefert. Die Formel auf dieser Seite ist die Aufschlag-Variante.

## Rechenbeispiel

Ein Packer wird bei einer Tätigkeit mit zwei Ablaufabschnitten über drei Zyklen gemessen. Jede Beobachtung hat einen Leistungsgrad.

| Ablaufabschnitt | Zyklus | Gemessen (s) | Leistungsgrad (%) | Gemessen × Leistungsgrad (s) |
|---|---|---|---|---|
| 1. Artikel greifen | 1 | 20 | 110 | 22,00 |
| 1. Artikel greifen | 2 | 22 | 100 | 22,00 |
| 1. Artikel greifen | 3 | 18 | 120 | 21,60 |
| 2. Verpacken und verschließen | 1 | 40 | 90 | 36,00 |
| 2. Verpacken und verschließen | 2 | 44 | 100 | 44,00 |
| 2. Verpacken und verschließen | 3 | 42 | 95 | 39,90 |

### Schritt 1: Normalzeit pro Ablaufabschnitt

- Abschnitt 1: (22,00 + 22,00 + 21,60) ÷ 3 = 21,87 s
- Abschnitt 2: (36,00 + 44,00 + 39,90) ÷ 3 = 39,97 s

### Schritt 2: Normale Zykluszeit

- 21,87 + 39,97 = 61,83 s

Vergleiche das mit dem einfachen Mittelwert der Messwerte: 20 s + 42 s = 62 s. Der Leistungsgrad verändert das Ergebnis hier nur wenig, weil sich hohe und niedrige Werte teilweise ausgleichen. Bei jemandem, der durchgehend schnell oder langsam arbeitet, ist der Abstand größer.

### Schritt 3: Zuschlag anwenden

Mit 15 % Zuschlag:

- 61,83 × 1,15 = 71,11 s

Die Vorgabezeit für einen Packzyklus beträgt rund 71,1 Sekunden. Mit dieser Vorgabe schafft eine Person etwa 50 Zyklen pro Stunde (3600 ÷ 71,11 = 50,6).

## Rechner

An interactive calculator is on the web page: https://apps.schimpf.es/time-study-stopwatch/de/standard-time-formula-example/

## Häufige Fehler

- Die Person bewerten statt das Tempo. Bewerte Geschwindigkeit und Einsatz der Arbeit, die du siehst. Bewerte jede Beobachtung, während du zusiehst.
- Den Leistungsgrad weglassen. Ohne ihn erhältst du den Durchschnitt, wie diese Person an diesem Tag gearbeitet hat, und noch keine Vorgabe.
- Zuschlagsarten mischen. Prüfe, ob dein Unternehmen den Zuschlag auf die Normalzeit oder auf die ganze Schicht bezieht, bevor du Zahlen vergleichst.
- Zu wenige Zyklen. Drei Zyklen genügen für eine Demo. Für eine echte Vorgabe nimm mehr Zyklen und schau dir die Streuung an. Eine große Standardabweichung zeigt, dass Methode oder Ablaufabschnitte noch nicht stabil sind.
- Unvollständige Zyklen messen. Zähle nur Zyklen, in denen jeder Ablaufabschnitt gemessen wurde, damit die Zykluszeit nicht zu niedrig ausfällt.

## In der App rechnen

Zeitstudie Stoppuhr wendet dieselbe Formel auf dem Ergebnis-Bildschirm an. Du legst die Arbeitselemente einmal an, tippst bei jedem Ende eines Elements auf den großen Rundenknopf und stellst pro Beobachtung einen Leistungsgrad ein. Gib den Zuschlag im Bildschirm zur Studieneinrichtung ein, dann zeigt die App Normalzeit pro Element, normale Zykluszeit und Vorgabezeit.

Mittelwert, Minimum, Maximum und Standardabweichung pro Element sind in der App enthalten. Leistungsgrad (50 bis 200 %), Zuschlag und Vorgabezeit gehören zu Zeitstudie Pro, einem Einmalkauf bei Google Play. Deine Daten bleiben auf dem Gerät, und mit dem CSV-Export überträgst du die Zahlen in eine Tabellenkalkulation.
