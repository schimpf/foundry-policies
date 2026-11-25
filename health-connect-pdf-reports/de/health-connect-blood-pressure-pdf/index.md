# Blutdruck-PDF aus Health Connect erstellen

> So machen Sie aus Blutdruck, Puls und Schlaf in Android Health Connect ein PDF für den Arzt, zum Teilen oder Drucken. Schritt für Schritt.

- Web: https://apps.schimpf.es/health-connect-pdf-reports/de/health-connect-blood-pressure-pdf/
- App: Health Reports: Werte als PDF, https://apps.schimpf.es/health-connect-pdf-reports/de/index.md
Viele Blutdruckmessgeräte, Uhren und Apps schreiben ihre Messwerte nach Health Connect, den Datenspeicher, der in Android eingebaut ist. Health Connect speichert die Daten und erstellt keinen Bericht, den Sie einer Ärztin oder einem Arzt geben können. Diese Seite zeigt, was Sie brauchen und wie aus den Daten ein übersichtliches PDF wird.

## Das brauchen Sie

- Ein Android-Handy. Ab Android 14 ist Health Connect enthalten. Auf Android 9 bis 13 installieren Sie die App Health Connect aus Google Play.
- Messwerte in Health Connect. Sie können von einem verbundenen Blutdruckmessgerät, einer Uhr oder einer Gesundheits-App kommen, die Health Connect unterstützt. Blutdruckwerte können Sie auch von Hand eintragen.
- Die App Health Connect PDF Reports.

## Schritt für Schritt

1. App öffnen und verbinden. Tippen Sie beim ersten Start auf Connect Health Connect und erlauben Sie die Berechtigungen. Die App liest Puls, Blutdruck und Schlaf. Sie schreibt nur Blutdruck, und zwar für Werte, die Sie von Hand eintragen.
2. Zeitraum wählen. Wählen Sie 7, 30 oder 90 Tage oder legen Sie eigene Daten fest. Die festen Zeiträume enden gestern, deshalb enthält der Bericht nur vollständige Tage.
3. Inhalt wählen. Blutdruck, Puls und Schlaf sind standardmäßig an. Schalten Sie ab, was Ihre Ärztin oder Ihr Arzt nicht braucht.
4. Namen eintragen, wenn Sie möchten. Das ist freiwillig. Ein Geburtsdatum ist nicht nötig. Der Name wird nur gespeichert, wenn Sie das wünschen.
5. Quellen prüfen. Wenn zwei Apps dieselben Werte aufzeichnen, legen Sie für jede Messgröße eine bevorzugte Quell-App fest oder lassen Sie Auto stehen.
6. Vorschau ansehen. Blättern Sie durch den Bericht, bevor Sie ihn senden.
7. Teilen oder drucken. Senden Sie das PDF über das normale Android-Menü zum Teilen per E-Mail oder Nachricht, oder nutzen Sie den Druckdialog.

## Das steht im Bericht

Der Bericht beginnt mit einer Zusammenfassung, danach folgt ein Abschnitt je Messgröße.

### Zusammenfassung

- Blutdruck: Durchschnitt, niedrigster und höchster Wert und Anzahl der Messungen.
- Puls: Durchschnitt, niedrigster und höchster Wert und der Durchschnitt des Ruhepulses. Bei Zeiträumen ab 14 Tagen die Veränderung des Ruhepulses zwischen den ersten 7 und den letzten 7 Tagen.
- Schlaf: Durchschnitt, kürzeste und längste Nacht.
- Blutdruckmessungen, gezählt nach AHA-Kategorie.

### Blutdruck-Seiten

Eine Tabelle mit jeder Messung samt Uhrzeit, Quell-App und AHA-Kategorie. Die Kategorien sind neutral benannt, zum Beispiel Normal, Elevated, Stage 1, Stage 2 und Above 180/120. Die Grenzen stehen in der [Blutdruck-Tabelle nach AHA](blood-pressure-categories-chart).

### Puls-Seiten

Eine Tabelle je Tag mit Ruhe-, Mindest-, Höchst- und Durchschnittswert, dazu ein Verlaufsdiagramm des Ruhepulses.

### Schlaf-Seiten

Eine Tabelle je Nacht mit Gesamtdauer und Schlafphasen, dazu eine Übersicht der Phasen als Durchschnitt pro Nacht. Der Schlafdurchschnitt auf der Zusammenfassung zählt die Zeit im Bett minus die Wachphase.

## So werden Doppelte behandelt

Speichern eine Messgerät-App und eine zweite App denselben Wert, sähen Sie ihn zweimal. Die App behandelt zwei Blutdruckmessungen als dasselbe Ereignis, wenn:

- sie aus verschiedenen Apps stammen,
- sie höchstens 2 Minuten auseinanderliegen und
- sowohl der systolische als auch der diastolische Wert um höchstens 2 mmHg abweichen.

Die Messung der bevorzugten Quelle bleibt erhalten. Der Bericht vermerkt, wie viele Doppelte zusammengeführt wurden. Schlafsitzungen verschiedener Apps werden zusammengeführt, wenn sie sich um mehr als die Hälfte der kürzeren Sitzung überlappen.

## Zur 30-Tage-Grenze

Health Connect gibt einer App nur die Daten der letzten 30 Tage, solange Sie den Zugriff auf den Verlauf nicht erlauben. Die App fragt nach dieser zusätzlichen Berechtigung nur, wenn der Zeitraum weiter als 30 Tage zurückreicht.

## Datenschutz

- Die App hat keine Internetberechtigung und kein Konto.
- Sie speichert keine Kopie Ihrer Gesundheitsdaten. Health Connect bleibt der einzige Ort der Daten.
- Das PDF entsteht im temporären Speicher und wird gelöscht, sobald Sie die Vorschau verlassen. Es geht nur dorthin, wohin Sie es senden.

## Gut zu wissen

- Ein Export ist ohne Zahlung möglich. Weitere Exporte brauchen einen einmaligen In-App-Kauf namens Unlimited reports (Unbegrenzte Berichte). Daten ansehen, Vorschau, Eintragen von Hand und das Widget brauchen keinen Kauf.
- Die App zeigt nur aufgezeichnete Werte. Sie stellt keine Diagnose und gibt keine medizinischen Ratschläge.
- Die App ist auf Englisch. Der Blutdruck wird in mmHg angegeben, das Datumsformat folgt Ihrem System.

## Tipps vor dem Termin

- Sehen Sie sich das PDF in der Vorschau an und prüfen Sie, ob der Zeitraum zu dem passt, was Ihre Ärztin oder Ihr Arzt verlangt hat.
- Tragen Sie ein paar Werte von Hand ein, wenn Ihr Messgerät nicht synchronisiert, damit das Protokoll keine Lücken hat.
- Bringen Sie den Bericht ausgedruckt mit oder halten Sie ihn auf dem Handy bereit.

Wenn Sie Zahlen zuerst selbst prüfen möchten, probieren Sie den [Blutdruck-Durchschnitt berechnen](average-blood-pressure-calculator).
