# WLAN-Kanäle und Frequenzen: Tabelle (2,4, 5, 6 GHz)

> WLAN-Frequenz in MHz in die Kanalnummer umrechnen, mit Tabelle für 2,4, 5 und 6 GHz und Tipps, wie du den besten Kanal wählst.

- Web: https://apps.schimpf.es/wifi-manager-and-test-tool/de/wifi-channel-and-frequency-chart/
- App: WLAN-Scanner & Netzwerktools, https://apps.schimpf.es/wifi-manager-and-test-tool/de/index.md
Jeder WLAN-Kanal ist eine Nummer, die für eine Mittenfrequenz in MHz steht. Diese Seite zeigt die Tabelle, die Formeln mit Rechenbeispielen und einen Umrechner, danach, wie du einen Kanal wählst.

## Formeln

Die Kanalnummer ergibt sich aus der Mittenfrequenz (f, in MHz). Der Abstand beträgt in allen drei Bändern 5 MHz. Das sind dieselben Formeln, die die App WLAN-Scanner & Netzwerktools verwendet.

| Band | Frequenzbereich (MHz) | Kanal |
|---|---|---|
| 2,4 GHz | 2412 bis 2472 | (f - 2407) / 5 |
| 2,4 GHz | 2484 | 14 |
| 5 GHz | 5160 bis 5885 | (f - 5000) / 5 |
| 6 GHz | 5955 bis 7115 | (f - 5950) / 5 |

Der Kanalplan selbst ist in IEEE Std 802.11 festgelegt (Ausgabe 2020 und ihre Änderungen). Welche Kanäle du nutzen darfst, hängt vom Land ab.

### Rechenbeispiele

1. 2437 MHz: (2437 - 2407) / 5 = 30 / 5 = Kanal 6, 2,4 GHz.
2. 5180 MHz: (5180 - 5000) / 5 = 180 / 5 = Kanal 36, 5 GHz.
3. 5955 MHz: (5955 - 5950) / 5 = 5 / 5 = Kanal 1, 6 GHz. Kanalnummern wiederholen sich im 6-GHz-Band, nenne deshalb immer das Band.
4. 2484 MHz ist ein Sonderfall: Kanal 14. Er ist nur in Japan erlaubt, und nur für das ältere 802.11b.

## Frequenz umrechnen

An interactive calculator is on the web page: https://apps.schimpf.es/wifi-manager-and-test-tool/de/wifi-channel-and-frequency-chart/

## Kanaltabelle 2,4 GHz

| Kanal | Mittenfrequenz (MHz) |
|---|---|
| 1 | 2412 |
| 2 | 2417 |
| 3 | 2422 |
| 4 | 2427 |
| 5 | 2432 |
| 6 | 2437 |
| 7 | 2442 |
| 8 | 2447 |
| 9 | 2452 |
| 10 | 2457 |
| 11 | 2462 |
| 12 | 2467 |
| 13 | 2472 |
| 14 | 2484 |

In den USA sind die Kanäle 1 bis 11 erlaubt. In Deutschland und den meisten anderen Ländern Europas sind es die Kanäle 1 bis 13.

## Beispiele für 5 GHz

| Kanal | Mittenfrequenz (MHz) |
|---|---|
| 36 | 5180 |
| 40 | 5200 |
| 44 | 5220 |
| 48 | 5240 |
| 100 | 5500 |
| 149 | 5745 |
| 165 | 5825 |

Einige 5-GHz-Kanäle (etwa 52 bis 144) teilen sich das Spektrum mit Radar. Dein Router muss dann eventuell den Kanal wechseln, was die Verbindung kurz unterbrechen kann.

## Beispiele für 6 GHz

| Kanal | Mittenfrequenz (MHz) |
|---|---|
| 1 | 5955 |
| 5 | 5975 |
| 37 | 6135 |
| 93 | 6415 |

6 GHz nutzen Geräte mit WiFi 6E und WiFi 7.

## Welchen Kanal soll ich nehmen?

- Im 2,4-GHz-Band ist jeder Kanal 20 MHz breit, die Kanäle liegen aber nur 5 MHz auseinander. Nachbarn auf den Kanälen 1 und 3 überlappen sich. Die einzigen drei Kanäle, die sich nicht überlappen, sind 1, 6 und 11. Nimm einen davon.
- 5 GHz und 6 GHz haben viel mehr Kanäle ohne Überlappung, Gedränge ist dort ein kleineres Problem.
- Wähle den Kanal, den deine Nachbarn am wenigsten nutzen. Ein Router auf "Auto" macht das meistens, aber nicht immer gut.
- Ein breiterer Kanal (40, 80 oder 160 MHz) bringt mehr Tempo, braucht aber mehr Platz und trifft auf mehr Störungen.
- Sieht ein Gerät dein 5-GHz-Netz nicht, prüfe, ob dein Router einen Kanal nutzt, den das Gerät unterstützt.

## Deinen Kanal unter Android finden

Der Bildschirm WiFi info in WLAN-Scanner & Netzwerktools zeigt Band, Kanal und Verbindungsgeschwindigkeit sowie den WLAN-Standard (WiFi 4, 5, 6 oder 7) deiner aktuellen Verbindung. Die App berechnet den Kanal mit den Formeln oben aus der Frequenz, die Android meldet. Android verlangt die Standortberechtigung, damit eine App den Netzwerknamen lesen darf. Die App nutzt oder speichert deinen Standort nicht.

Kombiniere das mit der [WLAN-Signalstärke-Tabelle](wifi-signal-strength-chart), um zu sehen, ob der Kanal oder die Signalstärke das Problem ist.
