# Schlummer-Rechner: Wie spät stehst du wirklich auf?

> Berechne, wie viele Minuten Schlummern dich kostet und wann der letzte Wecker klingelt. Mit Rechner und Rechenbeispiel.

- Web: https://apps.schimpf.es/alarm-clock/de/snooze-time-calculator/
- App: Wecker: Aufwach-Aufgaben, https://apps.schimpf.es/alarm-clock/de/index.md
Jedes Schlummern schiebt dein Aufstehen nach hinten. Diese Seite zeigt die Formel, ein Rechenbeispiel und einen kleinen Rechner, damit du siehst, was deine Schlummer-Gewohnheit wirklich kostet.

## Die Formel

Die Zeit, die du verlierst, folgt dieser Formel:

**Gesamtverzögerung = Schlummer-Intervall × Anzahl der Schlummer-Tipps**

Der letzte Wecker klingelt um:

**Letztes Klingeln = Weckzeit + Gesamtverzögerung**

Das gilt in der Praxis:

- Das Intervall zählt ab dem Moment, in dem du auf Schlummern tippst.
- Lässt du den Wecker eine Weile klingeln, bevor du tippst, ist die echte Verzögerung etwas länger als die Formel sagt.
- Die Formel gibt die Mindestverzögerung an. Sie stimmt genau, wenn du sofort auf Schlummern tippst.

## Rechner

An interactive calculator is on the web page: https://apps.schimpf.es/alarm-clock/de/snooze-time-calculator/

## Rechenbeispiel

Du stellst den Wecker auf 6:30 Uhr, mit 5 Minuten Intervall, und tippst 3-mal auf Schlummern.

1. Gesamtverzögerung = 5 min × 3 = 15 min.
2. Letztes Klingeln = 6:30 Uhr + 15 min = 6:45 Uhr.
3. Du stehst frühestens um 6:45 Uhr auf.

Derselbe Wecker mit 10 Minuten Intervall und 4-mal Schlummern:

1. Gesamtverzögerung = 10 min × 4 = 40 min.
2. Letztes Klingeln = 6:30 Uhr + 40 min = 7:10 Uhr.

Die Verzögerung für einige übliche Einstellungen:

| Intervall | Schlummern | Gesamtverzögerung |
| --- | --- | --- |
| 5 min | 1 | 5 min |
| 5 min | 3 | 15 min |
| 9 min | 3 | 27 min |
| 10 min | 4 | 40 min |
| 15 min | 5 | 75 min |
| 30 min | 10 | 300 min (5 h) |

## Das Ergebnis als Budget lesen

Wenn du um 7:00 Uhr aus dem Bett sein musst und schlummern willst, rechne rückwärts:

1. Wähle dein Intervall und die Anzahl der erwarteten Schlummer-Tipps.
2. Multipliziere sie, um die Gesamtverzögerung zu erhalten.
3. Ziehe die Verzögerung von 7:00 Uhr ab, um die Weckzeit zu erhalten.

Bei 5 Minuten Intervall und 3-mal Schlummern beträgt die Verzögerung 15 Minuten, also klingelt der Wecker um 6:45 Uhr. Das letzte Klingeln liegt bei 7:00 Uhr. Plane einen kleinen Puffer für die Zeit zwischen den Klingeln ein, denn du tippst nicht in der exakten Sekunde auf Schlummern, in der der Wecker startet.

## Setze ein Limit, mit dem du leben kannst

Unbegrenztes Schlummern hat keine Obergrenze, die Gesamtverzögerung also auch nicht. Ein Limit macht die Kosten im Voraus bekannt. Ist das Limit erreicht, bietet der Wecker kein Schlummern mehr an und du musst aufstehen.

## Schlummer-Einstellungen in Wecker

In Wecker stellst du beide Werte für jeden Wecker ein:

- **Intervall:** 1 bis 30 Minuten. Standard sind 5 Minuten.
- **Maximale Anzahl:** 0 bis 10 oder unbegrenzt. Standard sind 3.
- **0 Mal** schaltet Schlummern für diesen Wecker aus.
- Ein Chip auf dem Weckbildschirm zeigt, wie oft du geschlummert hast.
- Schlummern ist auf dem Weckbildschirm immer möglich, bis du dein Limit erreichst.
- Sobald eine Aufwach-Aufgabe gestartet ist, kannst du nicht mehr schlummern. Du schließt zuerst die Aufgabe ab.

Mit den Standardwerten sind es im schlimmsten Fall 5 × 3 = 15 Minuten zusätzlicher Schlaf, passend zum ersten Rechenbeispiel oben.

## Schlummern mit einer Aufgabe kombinieren

Willst du dir das Schlummern abgewöhnen, setze das Maximum auf eine kleine Zahl und füge eine Aufgabe hinzu. Wecker bietet vier: Rechenaufgaben, das Handy schütteln, einen QR-Code oder Barcode scannen und eine Anzahl Schritte gehen. Die Aufgabe lässt sich nicht überspringen. Schlägt sie dreimal fehl, bietet die App eine leichtere Rechenaufgabe an, damit du nie festhängst.

Wecker klingelt auf die Minute genau über die Wecker-Schnittstelle des Systems, nutzt die Weckerlautstärke und klingelt daher auch im Lautlos-Modus, und hat keine Internetberechtigung. Die App ist Open Source unter der GNU GPL v3 oder neuer. Stelle Intervall und Schlummer-Limit im Wecker-Editor ein.
