# Blutdruck-Durchschnitt berechnen, Rechner für Messwerte

> Blutdruck-Durchschnitt aus Ihren Messwerten berechnen, mit niedrigstem und höchstem Wert, AHA-Kategorie, Formel und Rechenbeispiel.

- Web: https://apps.schimpf.es/health-connect-pdf-reports/de/average-blood-pressure-calculator/
- App: Health Reports: Werte als PDF, https://apps.schimpf.es/health-connect-pdf-reports/de/index.md
Ärztinnen und Ärzte wollen meist den Durchschnitt mehrerer Messwerte von zu Hause sehen. Diese Seite bietet einen kleinen Rechner für eine Liste von Messwerten, danach folgen die Formel und ein Rechenbeispiel zum Nachrechnen.

## Rechner

Geben Sie pro Zeile einen Messwert als systolisch/diastolisch ein, zum Beispiel `122/78`. Nichts von dem, was Sie eingeben, verlässt Ihren Browser.

An interactive calculator is on the web page: https://apps.schimpf.es/health-connect-pdf-reports/de/average-blood-pressure-calculator/

## Die Formel

Systolischer und diastolischer Wert werden getrennt gemittelt.

- Durchschnitt systolisch = Summe aller systolischen Werte ÷ Anzahl der Messungen
- Durchschnitt diastolisch = Summe aller diastolischen Werte ÷ Anzahl der Messungen

Jedes Ergebnis wird auf die nächste ganze Zahl gerundet, bei ,5 wird aufgerundet. Niedrigste und höchste Messung sind die mit dem niedrigsten und dem höchsten systolischen Wert. Haben zwei Messungen denselben systolischen Wert, entscheidet der diastolische Wert.

Der Durchschnitt wird danach mit den AHA-Grenzen einer Kategorie zugeordnet.

| Kategorie | Systolisch | | Diastolisch |
|---|---|---|---|
| Normal | unter 120 | und | unter 80 |
| Erhöht (Elevated) | 120–129 | und | unter 80 |
| Stufe 1 (Stage 1) | 130–139 | oder | 80–89 |
| Stufe 2 (Stage 2) | 140 oder höher | oder | 90 oder höher |
| Über 180/120 (Above 180/120) | über 180 | und/oder | über 120 |

Die AHA ist die amerikanische Herzgesellschaft. Die deutsche Hochdruckliga und die europäische Leitlinie (ESC/ESH) benutzen andere Namen und Grenzen. Die App und diese Seite rechnen nach der AHA.

Quelle: Whelton PK, et al. *2017 ACC/AHA/AAPA/ABC/ACPM/AGS/APhA/ASH/ASPC/NMA/PCNA Guideline for the Prevention, Detection, Evaluation, and Management of High Blood Pressure in Adults*. Hypertension, 2018; 71(6): e13–e115.

## Rechenbeispiel

Sieben Morgenmessungen in einer Woche:

| Tag | Messwert |
|---|---|
| Montag | 128/82 |
| Dienstag | 122/78 |
| Mittwoch | 135/85 |
| Donnerstag | 126/80 |
| Freitag | 131/84 |
| Samstag | 120/76 |
| Sonntag | 124/79 |

### Schritt 1: systolische Werte addieren

128 + 122 + 135 + 126 + 131 + 120 + 124 = 886

### Schritt 2: diastolische Werte addieren

82 + 78 + 85 + 80 + 84 + 76 + 79 = 564

### Schritt 3: durch die Anzahl der Messungen teilen

- 886 ÷ 7 = 126,57, gerundet 127
- 564 ÷ 7 = 80,57, gerundet 81

Der Durchschnitt ist 127/81.

### Schritt 4: niedrigsten und höchsten Wert finden

- Niedrigster systolischer Wert: 120/76
- Höchster systolischer Wert: 135/85

### Schritt 5: den Durchschnitt einer Kategorie zuordnen

Systolisch 127 liegt in der Zeile 120–129. Diastolisch 81 liegt in der Zeile 80–89. Die beiden Zahlen zeigen auf verschiedene Zeilen, deshalb gilt die höhere Kategorie: Stufe 1.

Dieselbe Woche läge in Erhöht, wenn der diastolische Durchschnitt 79 oder niedriger gewesen wäre. Ein oder zwei Punkte können einen Durchschnitt über eine Grenze schieben, deshalb lohnt der Blick auf die ganze Liste und auf den Durchschnitt.

## Kategorie des Durchschnitts und Kategorie jeder Messung

Der Rechner bildet zuerst den Durchschnitt und ordnet danach die Kategorie zu. Sie können auch jede Messung einzeln einordnen. Im Beispiel:

- Stufe 1: 128/82, 135/85, 126/80, 131/84 (4 Messungen)
- Erhöht: 122/78, 120/76, 124/79 (3 Messungen)
- Normal, Stufe 2 und Über 180/120: 0 Messungen

Die Kategorie des Durchschnitts und die Anzahl je Kategorie können voneinander abweichen. Beides ist für den Arztbesuch nützlich.

## Tipps für einen brauchbaren Durchschnitt

- Messen Sie an mehreren Tagen.
- Nehmen Sie denselben Arm, dieselbe Manschette und eine ähnliche Tageszeit.
- Tragen Sie jede gültige Messung ein. Wer die hohen Werte weglässt, bekommt einen wertlosen Durchschnitt.
- Mitteln Sie Messungen verschiedener Geräte nicht ohne Vermerk. Manschetten können um einige mmHg abweichen.

Ein Rechner kann nicht beurteilen, ob ein Wert für Sie ein Problem ist. Nehmen Sie die Liste und den Durchschnitt zu Ihrer Ärztin oder Ihrem Arzt mit.

## Ohne Rechnen mit der App

Health Connect PDF Reports für Android übernimmt diese Arbeit für die Messwerte in Health Connect. Die Zusammenfassung zeigt Durchschnitt, niedrigsten und höchsten Blutdruck, den Verlauf des Ruhepulses, die durchschnittliche Schlafdauer und die Anzahl der Messungen je AHA-Kategorie. Die Detailseiten listen jede Messung mit Uhrzeit und Quell-App. Der Durchschnitt entsteht wie oben: systolisch und diastolisch getrennt gemittelt und auf ganze Zahlen gerundet. Messungen, die zwei Apps für dasselbe Ereignis gespeichert haben, werden vorher zusammengeführt und zählen einmal.

Sie können in der App auch einen Wert von Hand eintragen. Er wird in Health Connect gespeichert. Die App ist auf Englisch und nennt die Kategorien dort Normal, Elevated, Stage 1, Stage 2 und Above 180/120. Sie zeigt nur aufgezeichnete Werte und stellt keine Diagnose und gibt keine medizinischen Ratschläge.

Siehe auch: [Blutdruck-Tabelle nach AHA](blood-pressure-categories-chart) und [Blutdruck-PDF aus Health Connect erstellen](health-connect-blood-pressure-pdf).
