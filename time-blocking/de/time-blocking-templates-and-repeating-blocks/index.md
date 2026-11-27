# Zeitblock-Vorlagen und wiederkehrende Blöcke in der App

> Tabelle mit Vorlagen für Zeitblöcke samt Dauer und wie tägliche, Mo-Fr- und frei gewählte Wiederholungen in der Time-Blocking-App funktionieren.

- Web: https://apps.schimpf.es/time-blocking/de/time-blocking-templates-and-repeating-blocks/
- App: Time Blocking Tagesplaner, https://apps.schimpf.es/time-blocking/de/index.md
## Warum Blöcke wiederverwenden

An den meisten Tagen kommen dieselben Blöcke vor: ein Planungsslot, das Mittagessen, ein Tagesrückblick. Sie jeden Tag neu anzulegen dauert länger als das Planen selbst. Zwei Funktionen übernehmen das: Vorlagen für Blöcke, die du von Hand hinzufügst, und wiederkehrende Blöcke für Blöcke, die nach einem Muster zurückkommen.

Diese Seite nennt Vorlagen mit Dauer und zeigt, wie jede Wiederholungsoption in Time Blocking funktioniert.

## Vorlagen mit Dauer

Eine Vorlage in der App enthält einen Namen, eine Dauer und eine Farbe. Sie hat keine Startzeit, die wählst du beim Hinzufügen.

| Vorlage | Dauer | Wochensumme bei einmal pro Wochentag |
|---|---|---|
| Tag planen | 15m | 1h 15m |
| Konzentrierte Arbeit | 2h | 10h |
| E-Mails | 30m | 2h 30m |
| Mittagessen | 1h | 5h |
| Telefonate | 45m | 3h 45m |
| Rückblick und Feierabend | 15m | 1h 15m |
| Sport | 1h | 5h |

Die Wochensumme ist die Dauer mal 5. Beispiel: 45 Minuten mal 5 sind 225 Minuten, also 3h 45m.

Nimm eine Farbe pro Art von Arbeit. Die Palette hat 12 Farben: Indigo, Blau, Cyan, Türkis, Grün, Limette, Bernstein, Orange, Koralle, Rot, Pink und Violett.

## Vorlage anlegen und nutzen

1. Öffne den Bereich Templates, um Vorlagen anzulegen, zu bearbeiten oder zu löschen. Beim Löschen fragt die App nach.
2. Oder bearbeite einen bereits gesetzten Block und speichere ihn über "Save as template" als Vorlage.
3. Wenn du einen Block hinzufügst und mindestens eine Vorlage existiert, bietet eine Auswahl "Block" (leer) oder eine deiner Vorlagen an.
4. Wähle eine Vorlage und lege dann die Startzeit fest.

Die App speichert die Dauer, daher erzeugt eine Vorlage "Telefonate" mit 45 Minuten immer einen Block von 45 Minuten.

## Wiederkehrende Blöcke

Ein Block kann sich wiederholen. Das Feld "Repeat" hat vier Auswahlmöglichkeiten:

- **Never**: ein einzelner Block.
- **Daily**: jeden Tag ab dem Startdatum.
- **Weekdays**: Montag bis Freitag (der Samstag zählt nicht dazu).
- **Custom**: die Wochentage, die du ankreuzt, zum Beispiel Montag, Mittwoch und Freitag.

Du kannst ein Enddatum setzen. Der Block erscheint an jedem passenden Tag vom Startdatum bis einschließlich zum Enddatum.

### Rechenbeispiel

Ein Block "Tag planen" von 15 Minuten um 08:00, der sich an Wochentagen wiederholt, an einem Montag beginnt und am Freitag der Folgewoche endet, erscheint an 10 Tagen (zwei Wochen von Montag bis Freitag). Das sind 10 mal 15 Minuten, also insgesamt 2h 30m Planung.

Eine eigene Wiederholung an Montag, Mittwoch und Freitag ergibt für dieselben zwei Wochen 6 Termine.

## Einen Termin oder alle ändern

Wenn du einen wiederkehrenden Block bearbeitest, verschiebst, in der Länge änderst oder löschst, fragt die App: "This occurrence" oder "All occurrences".

- **This occurrence** ändert nur diesen Tag. Der Block wird an diesem Tag zu einem normalen Einzelblock, und die Serie läuft drumherum weiter.
- **All occurrences** ändert die ganze Serie.

Diese Regeln solltest du kennen:

- Verschiebst du einen Termin auf einen anderen Tag, betrifft das nur diesen Termin. Eine ganze Serie kann den Tag nicht wechseln.
- Stellst du eine Serie an einem Termin auf Never, endet die Serie am Vortag, und dieser Tag wird zu einem Einzelblock.
- Löschst du einen Termin, entfällt dieser Tag, und der Rest der Serie bleibt.

## Tagesaktionen und Wiederholungen

- **Tag duplizieren** kopiert ihn als Einzelblöcke auf ein anderes Datum. Eine Serie, die am Zieldatum schon läuft, wird nicht doppelt angelegt.
- **Tag leeren** löscht die Einzelblöcke. Wiederkehrende Blöcke entfallen nur für diesen Tag und kehren am nächsten passenden Tag zurück.

## Was passt wann

| Du willst | Nimm |
|---|---|
| Denselben Block zur selben Zeit an jedem Wochentag | Repeat: Weekdays |
| Denselben Block an drei festen Tagen | Repeat: Custom |
| Einen Block mit fester Dauer, aber an jedem Tag zu anderer Zeit | Vorlage |
| Einen Tag auf ein neues Datum kopieren | Tag duplizieren |

## Grenzen

- Vorlagen haben keine Startzeit und keine Notiz.
- Die App hat keine Erinnerungen und keine Benachrichtigungen, ein wiederkehrender Block meldet sich also nicht.
- Ein Update von der ersten Datenbankversion entfernt alte Vorlagen für ganze Tage.

Die Schritte für einen vollständigen Tag stehen unter [Tag mit Zeitblöcken planen](../how-to-time-block-your-day/).

Time Blocking läuft offline und speichert alles auf deinem Gerät. Die Oberfläche ist derzeit auf Englisch, deshalb stehen die Bezeichnungen der App hier auf Englisch.
