# WLAN-Signalstärke-Tabelle (dBm und Signalqualität)

> Was WLAN-Werte von -30 bis -100 dBm bedeuten: Tabelle, Schnellprüfung und was du bei schwachem Signal tun kannst.

- Web: https://apps.schimpf.es/wifi-manager-and-test-tool/de/wifi-signal-strength-chart/
- App: WLAN-Scanner & Netzwerktools, https://apps.schimpf.es/wifi-manager-and-test-tool/de/index.md
Die WLAN-Signalstärke wird als RSSI in dBm angegeben. Die Zahl ist negativ, und je näher an null, desto stärker das Signal. Diese Seite zeigt eine Tabelle, ein kleines Prüfwerkzeug und ein paar Lösungen.

## WLAN-Signalstärke-Tabelle

| Signal (dBm) | Qualität | Balken (von 4) | Was du erwarten kannst |
|---|---|---|---|
| -55 oder höher | Ausgezeichnet | 4 | Volle Geschwindigkeit. Videoanrufe und Streaming laufen stabil. |
| -56 bis -67 | Gut | 3 | Zuverlässig für Streaming, Anrufe und Surfen. |
| -68 bis -75 | Mittel | 2 | Es funktioniert, aber das Tempo sinkt und Anrufe können stocken. |
| -76 bis -99 | Schwach | 1 | Langsame Seiten, Abbrüche und lange Wartezeiten. |
| -100 oder niedriger | Kein Signal | 0 | Nicht nutzbar. |

Diese Bereiche verwendet die App WLAN-Scanner & Netzwerktools. Andere Tools ziehen die Grenzen ein paar dBm weiter oben oder unten, sieh sie deshalb als Richtwert.

## So liest du dBm

- dBm ist eine logarithmische Skala. Jede Änderung um 3 dBm verdoppelt oder halbiert die Leistung ungefähr.
- -50 dBm hat etwa 1000-mal mehr Leistung als -80 dBm. Ein Abfall von -55 auf -75 ist ein Verlust um den Faktor 100.
- Eine Änderung von 1 oder 2 dBm ist Rauschen. So viel schwankt das Signal, wenn du dich drehst oder das Handy bewegst.
- Der Wert ist das, was dein Handy vom Router empfängt. Er sagt nichts darüber, wie gut dein Router dein Handy hört.

### Beispiel

Du misst -62 dBm im Wohnzimmer und -79 dBm im Schlafzimmer.

1. Wohnzimmer: -62 liegt zwischen -56 und -67, also Gut.
2. Schlafzimmer: -79 liegt zwischen -76 und -99, also Schwach.
3. Der Unterschied beträgt 17 dBm, das sind etwa 50-mal weniger Leistung im Schlafzimmer (17 / 10 = 1,7, und 10^1,7 ist etwa 50).

Kümmere dich zuerst um das Schlafzimmer.

## Wert prüfen

An interactive calculator is on the web page: https://apps.schimpf.es/wifi-manager-and-test-tool/de/wifi-signal-strength-chart/

## Was dein Signal schwächt

- Entfernung. Das Signal fällt in den ersten Metern schnell ab, danach langsamer.
- Wände. Ziegel, Beton und Stein dämpfen stärker als Trockenbau. Metall und Spiegel dämpfen am stärksten.
- Band. 5 GHz und 6 GHz reichen weniger weit als 2,4 GHz und werden von Wänden stärker gebremst.
- Störungen. Nachbarnetze auf demselben Kanal, Mikrowellen und schnurlose Telefone (zum Beispiel DECT) erzeugen Rauschen. Mit der [WLAN-Kanaltabelle](wifi-channel-and-frequency-chart) findest du einen ruhigeren Kanal.
- Standort des Routers. Ein Router auf dem Boden, im Schrank oder in einer Ecke versorgt weniger vom Zuhause.

## So verbesserst du ein schwaches Signal

1. Stelle den Router an eine zentrale, höhere und freie Stelle.
2. Geh in den schwachen Raum und beobachte den Wert live, während du Router oder Handy bewegst.
3. Wechsle auf einen weniger belegten Kanal.
4. Nutze im 2,4-GHz-Band Kanal 1, 6 oder 11, damit du die Nachbarn nicht stärker überlappst als nötig.
5. Bleibt ein Raum schwach, ergänze einen Access Point oder einen Mesh-Knoten auf halbem Weg dorthin, wenn möglich per Kabel angebunden.

## Auf dem Handy messen

Der Bildschirm WiFi info in WLAN-Scanner & Netzwerktools zeigt dein aktuelles Signal in dBm mit dem Qualitätsnamen und der Vier-Balken-Anzeige aus der Tabelle oben. Außerdem zeigt er Band, Kanal, Verbindungsgeschwindigkeit und WLAN-Standard. Android verlangt die Standortberechtigung, bevor eine App den Netzwerknamen lesen darf. Die App nutzt oder speichert deinen Standort nicht.

Geh mit geöffnetem Bildschirm durch die Wohnung und notiere den Wert in jedem Raum. Alles bleibt auf deinem Handy.

## Signal und Geschwindigkeit

Ein starkes Signal ist für Tempo nötig, aber die beiden Werte sind nicht dasselbe. Die Verbindungsgeschwindigkeit hängt vom WLAN-Standard, der Kanalbreite und der Zahl der Geräte ab, die sich den Kanal teilen. Ein Signal von -50 dBm auf einem vollen Kanal kann trotzdem langsam sein. Ist das Signal gut und die Verbindung trotzdem langsam, prüfe den Kanal und starte einen Ping, um die Latenz zu sehen.
