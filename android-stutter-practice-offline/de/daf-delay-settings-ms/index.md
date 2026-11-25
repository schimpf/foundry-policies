# DAF-Verzögerung in ms einstellen: Werte und Beispiel

> Wie viel Verzögerung bei DAF (verzögertes Hören) gegen Stottern? Handy-Latenz, Formel, Rechenbeispiel und Rechner.

- Web: https://apps.schimpf.es/android-stutter-practice-offline/de/daf-delay-settings-ms/
- App: Stottern üben: DAF, https://apps.schimpf.es/android-stutter-practice-offline/de/index.md
Bei verzögerter auditiver Rückkopplung (DAF) hörst du deine eigene Stimme einen Bruchteil einer Sekunde zu spät. Die Verzögerung wird in Millisekunden (ms) eingestellt. Auf dem Handy erzeugt der Audioweg selbst schon eine Verzögerung, deshalb ist die eingestellte Zahl nicht immer die Verzögerung, die du hörst. Diese Seite zeigt die Formel und zwei Rechenbeispiele.

## Was DAF ist

Du sprichst ins Mikrofon, und die App spielt deine Stimme nach kurzer Verzögerung über die Kopfhörer ab. DAF ist ein Verfahren aus der Sprachtherapie bei Stottern. Wie stark es hilft, ist von Mensch zu Mensch verschieden, und die passende Einstellung findest du am besten mit einer Logopädin oder einem Logopäden. Diese Seite ist eine allgemeine Information und keine medizinische Beratung.

## Typische Verzögerungswerte

In Stutter Practice stellst du die Verzögerung von 25 bis 250 ms ein. Der Startwert ist 75 ms, dazu gibt es vier Schnellwahlen:

| Schnellwahl | Verzögerung |
|---|---|
| 1 | 50 ms |
| 2 | 75 ms (auch der Startwert) |
| 3 | 100 ms |
| 4 | 150 ms |

Ändere den Wert in kleinen Schritten und behalte, was sich angenehm anfühlt.

## Warum das Handy Verzögerung hinzufügt

Jedes Android-Handy hat zwischen Mikrofon und Kopfhörer eine gewisse Verzögerung. Sie entsteht im Eingangspuffer, in der Verarbeitung und im Ausgangspuffer und heißt Geräte-Latenz. Stellst du in einer App, die sie ignoriert, 100 ms ein, hörst du unter Umständen 100 ms plus die Geräte-Latenz.

Stutter Practice liest die Geräte-Latenz bei einer kurzen Kalibrierung aus und lässt dich sie feinjustieren, indem du zu Klicks mittippst. Der gespeicherte Wert ist:

- Geräte-Latenz = gemessene Basis-Latenz + Feinabstimmung
- Die Feinabstimmung ist die mittlere Verspätung deiner letzten Taps (Median), zwischen 0 und 60 ms.

## Die Formel

- Verzögerung, die die App hinzufügt = Zielverzögerung − Geräte-Latenz
- Der Wert fällt nie unter null.
- Liegt das Ziel unter der Geräte-Latenz, hörst du allein die Geräte-Latenz, und die App zeigt eine Warnung.

## Rechenbeispiele

Angenommen, die Kalibrierung hat eine Geräte-Latenz von 40 ms ergeben.

1. Du willst 100 ms. Die App fügt 100 − 40 = 60 ms hinzu. Du hörst insgesamt etwa 100 ms.
2. Du willst 75 ms. Die App fügt 75 − 40 = 35 ms hinzu.
3. Du willst 25 ms. 25 − 40 ist negativ, also fügt die App 0 ms hinzu. Du hörst etwa 40 ms, mehr als gewünscht. Die App warnt dich, dass deine Einstellung unter der Geräteverzögerung liegt.

Nun angenommen, die Geräte-Latenz beträgt 70 ms, was bei manchen Handys vorkommt:

| Ziel | Von der App hinzugefügt | Zu hören (etwa) |
|---|---|---|
| 50 ms | 0 ms | 70 ms |
| 75 ms | 5 ms | 75 ms |
| 100 ms | 30 ms | 100 ms |
| 150 ms | 80 ms | 150 ms |

## Rechner

An interactive calculator is on the web page: https://apps.schimpf.es/android-stutter-practice-offline/de/daf-delay-settings-ms/

## Kopfhörer sind wichtig

- Nimm kabelgebundene oder USB-Kopfhörer. Sie fügen die geringste Verzögerung hinzu und halten sie stabil.
- Bluetooth fügt zusätzliche Verzögerung hinzu, die von Gerät zu Gerät schwankt. Die App zeigt deshalb eine Warnung, wenn ein Bluetooth-Ausgang aktiv ist.
- Auch der Handylautsprecher wird gekennzeichnet, weil er ebenfalls zusätzlich verzögert.
- Die Kalibrierung wird für den Ausgang gespeichert, den du benutzt hast. Wechselst du die Kopfhörer, kalibriere neu.

## Üben mit Stutter Practice

Stutter Practice ist eine Android-App für DAF, Sprechen im Takt und Übungen zum weichen Stimmeinsatz. Sie funktioniert ohne Internetverbindung, hat keine Netzwerkberechtigung und verarbeitet deine Stimme live, ohne sie aufzunehmen. Die Verzögerung änderst du bei laufendem DAF per Schieberegler, Plus- und Minus-Tasten oder Schnellwahl. DAF lässt sich auch mit den Vorlesetexten kombinieren.
