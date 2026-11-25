# Wasserzähler Kleingarten: Kosten berechnen mit Beispiel

> Wasser- und Stromkosten im Kleingartenverein aus dem Zählerstand berechnen: Formel, Grundgebühr, Rechenbeispiel und Umgang mit unplausiblen Ständen.

- Web: https://apps.schimpf.es/german-allotment-club-ledger/de/allotment-water-meter-cost-calculation/
- App: Kleingarten-Kasse für Vereine, https://apps.schimpf.es/german-allotment-club-ledger/de/index.md
In vielen Kleingartenvereinen hat jede Parzelle einen eigenen Wasserzähler, manche auch einen Stromzähler. Der Kassenwart liest die Zähler einmal im Jahr ab und rechnet jeder Parzelle ihren Verbrauch ab. Diese Seite zeigt die Formel, ein Rechenbeispiel und Regeln für Zählerstände, die nicht stimmen können.

## Die Formel

**Verbrauch = Endstand − Anfangsstand**

**Kosten = Verbrauch × Preis pro Einheit + Grundgebühr**

- Wasser wird in Kubikmetern (m³) abgerechnet, Strom in Kilowattstunden (kWh).
- Den Preis pro Einheit legt der Verein fest. Er richtet sich meist nach dem, was der Verein an den Versorger zahlt, plus Kosten für Zähler und Wartung.
- Die Grundgebühr ist optional. Sie ist ein fester Betrag pro Parzelle und Jahr für die Fixkosten, egal wie hoch der Verbrauch ist.

### Beispiel: eine Parzelle, ein Jahr

- Anfangsstand, 1. Januar: 1.204 m³
- Endstand, 31. Dezember: 1.236,5 m³
- Verbrauch: 1.236,5 − 1.204 = **32,5 m³**
- Preis: 4,20 € pro m³
- Grundgebühr: 12,00 €

Kosten: 32,5 × 4,20 € = 136,50 €, dazu 12,00 € = **148,50 €**.

Die Preise oben sind nur Beispiele. Nehmen Sie die Zahlen Ihres Vereins.

## Der Endstand ist der nächste Anfangsstand

Der Endstand eines Jahres ist der Anfangsstand des nächsten. Passen beide nicht zusammen, ist zwischen den Ablesungen etwas passiert: ein Zahlendreher, ein Zählertausch oder der falsche Zähler wurde abgelesen. Prüfen Sie das vor der Abrechnung.

| Situation | Was zu prüfen ist |
|---|---|
| Endstand kleiner als Anfangsstand | Zahlendreher, Zählertausch oder Zähler über die Höchstzahl hinausgelaufen |
| Anfangsstand weicht vom Endstand des Vorjahres ab | Zahlendreher oder Zähler wurde ausgetauscht |
| Sehr hoher Verbrauch | Leck oder ein Schlauch, der gelaufen ist |

### Zählertausch

Bei einem neuen Zähler beginnt die Zählung bei oder nahe null, die einfache Subtraktion ergibt also eine negative Zahl. Rechnen Sie keinen negativen Betrag ab. Setzen Sie ihn auf null und rechnen Sie den echten Verbrauch aus dem letzten Stand des alten und dem ersten Stand des neuen Zählers ab, den Sie von Hand notieren. Kleingarten-Kasse rechnet ein negatives Ergebnis als null ab und erzeugt deshalb nie versehentlich eine Gutschrift.

## Wenn der Pächter mitten im Jahr wechselt

Wasser und Strom gehören zur Parzelle und werden wie die Pacht monatsgenau aufgeteilt. Am Übergabetag wird meist nicht abgelesen, deshalb teilt der Verein den Jahresbetrag nach den Monaten, in denen jeder Pächter die Parzelle hatte. Die Grundgebühr teilen beide Pächter auf die gleiche Weise.

Liest Ihr Verein am Übergabetag ab, rechnen Sie jedem Pächter seinen eigenen Verbrauch ab. Legen Sie eine Regel fest und schreiben Sie sie in die Satzung, damit es keinen Streit gibt.

### Beispiel: Wechsel nach Juni

- Jahreskosten: 148,50 €
- Pächter A: Januar bis Juni, 6 Monate: 148,50 € × 6 ÷ 12 = 74,25 €
- Pächter B: Juli bis Dezember, 6 Monate: 148,50 € − 74,25 € = 74,25 €

Wie bei ungleichen Anteilen gerundet wird, steht unter [Pachtzins im Kleingarten berechnen](kleingarten-pacht-berechnen).

## Checkliste für den Ablesetag

1. Lesen Sie alle Zähler am selben Tag ab, gegen Jahresende.
2. Notieren Sie die Zahl mit allen Stellen nach dem Komma.
3. Fotografieren Sie das Zifferblatt, wenn möglich.
4. Vergleichen Sie jeden Anfangsstand mit dem Endstand des Vorjahres.
5. Gehen Sie jeder Parzelle nach, deren Endstand unter dem Anfangsstand liegt.
6. Rechnen Sie erst nach diesen Prüfungen ab.

## In der App

Kleingarten-Kasse hat eine schnelle Erfassung für Zählerstände, Parzelle für Parzelle in Reihenfolge. Die App speichert Stände mit drei Nachkommastellen, 1.236,5 ist also exakt. Sie warnt, wenn ein Endstand unter dem Anfangsstand liegt oder ein Anfangsstand nicht zum letzten Endstand passt. Die Warnungen verhindern das Speichern nicht, denn ein Zählertausch ist ein berechtigter Grund.

Sie legen den Preis pro m³ oder kWh und eine optionale Grundgebühr einmal pro Jahr fest. Die App fügt dann die Wasser- und Stromzeilen zu den Kosten jeder Parzelle hinzu, teilt sie bei Pächterwechsel nach Monaten und setzt sie auf die Pachtrechnung als PDF.

Die App hat keine Internet-Berechtigung, Zählerstände und Preise bleiben auf Ihrem Gerät.
