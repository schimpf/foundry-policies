# Durchschnitts-BPM einer Übungseinheit berechnen

> So berechnest du das zeitgewichtete Durchschnittstempo, wenn du beim Üben das Tempo änderst. Mit Rechenbeispiel und typischen Fehlern.

- Web: https://apps.schimpf.es/metronome-and-practice-log/de/average-bpm-practice-session/
- App: Metronom & Übungsprotokoll, https://apps.schimpf.es/metronome-and-practice-log/de/index.md
Wenn du das Metronom-Tempo beim Üben änderst, ist eine Zahl für die ganze Einheit praktisch: das Durchschnitts-BPM. Der einfache Mittelwert der Tempi, die du benutzt hast, ist falsch. Du brauchst den zeitgewichteten Durchschnitt.

## Die Formel

**Durchschnitts-BPM = (BPM1 x Zeit1 + BPM2 x Zeit2 + ...) / (Zeit1 + Zeit2 + ...)**

Jedes Tempo zählt so stark, wie lange du dabei geblieben bist. Nimm für alle Teile dieselbe Zeiteinheit. Minuten oder Sekunden funktionieren beide.

Diese Formel nutzt auch Metronom & Übungsprotokoll. Während du spielst, addiert die App Tempo mal vergangene Zeit und teilt beim Pausieren durch die Gesamtzeit.

## Rechenbeispiel

Du übst ein Stück 20 Minuten lang:

1. 10 Minuten bei 80 BPM.
2. 5 Minuten bei 100 BPM.
3. 5 Minuten bei 120 BPM.

Schritt für Schritt:

1. Multipliziere jedes Tempo mit seiner Zeit: 80 x 10 = 800, 100 x 5 = 500, 120 x 5 = 600.
2. Addiere die Ergebnisse: 800 + 500 + 600 = 1.900.
3. Addiere die Zeiten: 10 + 5 + 5 = 20 Minuten.
4. Teile: 1.900 / 20 = 95 BPM.

```
80 BPM  |##########  10 Min.
100 BPM |#####        5 Min.
120 BPM |#####        5 Min.
Durchschnitt: 95 BPM
```

Der einfache Mittelwert aus 80, 100 und 120 ist 100. Das ist zu hoch, weil du die Hälfte der Einheit im langsamsten Tempo verbracht hast.

## Durchschnitts-BPM und letztes BPM sind verschieden

Eine Einheit hat zwei Tempowerte, die sich zu merken lohnen:

- Das letzte BPM ist das Tempo, bei dem du aufgehört hast. Im Beispiel sind es 120.
- Das Durchschnitts-BPM ist der zeitgewichtete Wert. Im Beispiel sind es 95.

Das letzte BPM zeigt, wo du gelandet bist. Das Durchschnitts-BPM zeigt, wie du gearbeitet hast. Wenn du langsam einspielst und schnell endest, wirkt das letzte BPM hoch, während der Durchschnitt die ganze Einheit abdeckt. Metronom & Übungsprotokoll speichert beide Werte für jede Einheit.

## Ein zweites Beispiel mit Sekunden

Du spielst 45 Sekunden bei 60 BPM und dann 15 Sekunden bei 90 BPM.

1. 60 x 45 = 2.700.
2. 90 x 15 = 1.350.
3. Summe: 4.050, geteilt durch 60 Sekunden = 67,5 BPM.

## Typische Fehler

- Die Tempi ohne Gewichtung mitteln. Gewichte immer nach Zeit.
- Pausen mitzählen. Zeit bei gestopptem Metronom gehört nicht in die Rechnung. Die App startet eine Einheit, wenn du Play drückst, und beendet sie, wenn du pausierst. Es zählt nur die Spielzeit.
- Einheiten mischen. Nimm nicht für einen Teil Minuten und für einen anderen Sekunden.
- Von einer späten Tempoänderung viel erwarten. Eine Änderung kurz vor Schluss bewegt den Durchschnitt kaum, und das ist richtig so.

## Mit dem Durchschnitts-BPM den Fortschritt verfolgen

Eine Einheit sagt wenig. Protokolliere deshalb dasselbe Stück über mehrere Wochen und sieh zu, wie der Durchschnitt steigt:

| Woche | Durchschnitts-BPM |
|---|---|
| 1 | 72 |
| 2 | 80 |
| 3 | 88 |
| 4 | 96 |

Etwa 8 BPM mehr pro Woche sind ein klarer Trend. Wenn die Zahl stockt, bleib noch ein paar Tage im selben Tempo, bevor du weitergehst.

## Was die App aufzeichnet

- Eine Einheit beginnt, wenn du Play drückst, und endet, wenn du pausierst.
- Einheiten unter 30 Sekunden werden ignoriert, damit ein kurzer Tempotest das Protokoll nicht füllt.
- Jede Einheit speichert ihr Stück (oder „General“), die Taktart, das letzte Tempo und das zeitgewichtete Durchschnittstempo.
- Du kannst jede Einheit bearbeiten oder löschen, mit Rückgängig.
- Jeder Tag mit mindestens einer Minute Üben zählt für deine tägliche Serie.
- Diagramme zum Tempofortschritt je Stück und die 12-Wochen-Ansicht gehören zum Pro-Kauf. Das 7-Tage-Diagramm funktioniert ohne.

Alle Daten bleiben auf deinem Gerät. Die App hat keine Internetberechtigung und kein Konto.

## In der App ausprobieren

Metronom & Übungsprotokoll ist ein Android-Metronom, das deine Übezeit automatisch protokolliert, du musst also nicht von Hand rechnen. Such die App bei Google Play.
