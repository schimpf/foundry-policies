# WiFi Channel and Frequency Chart (2.4, 5, 6 GHz)

> Convert a WiFi frequency in MHz to its channel number, with a chart for 2.4, 5 and 6 GHz and how to pick a channel.

- Web: https://apps.schimpf.es/wifi-manager-and-test-tool/wifi-channel-and-frequency-chart/
- App: WiFi Scanner & Network Tools, https://apps.schimpf.es/wifi-manager-and-test-tool/index.md
Every WiFi channel is a number that stands for a center frequency in MHz. This page gives the chart, the formulas with worked examples and a converter, then shows how to pick a channel.

## Formulas

The channel number comes from the center frequency (f, in MHz). The spacing is 5 MHz in all three bands. These are the same formulas the app WiFi Scanner & Network Tools uses.

| Band | Frequency range (MHz) | Channel |
|---|---|---|
| 2.4 GHz | 2412 to 2472 | (f - 2407) / 5 |
| 2.4 GHz | 2484 | 14 |
| 5 GHz | 5160 to 5885 | (f - 5000) / 5 |
| 6 GHz | 5955 to 7115 | (f - 5950) / 5 |

The channel plan itself is defined in IEEE Std 802.11 (the 2020 revision and its amendments). Which channels you may use depends on your country.

### Worked examples

1. 2437 MHz: (2437 - 2407) / 5 = 30 / 5 = channel 6, 2.4 GHz.
2. 5180 MHz: (5180 - 5000) / 5 = 180 / 5 = channel 36, 5 GHz.
3. 5955 MHz: (5955 - 5950) / 5 = 5 / 5 = channel 1, 6 GHz. Channel numbers repeat in 6 GHz, so always name the band.
4. 2484 MHz is a special case: channel 14. It is only allowed in Japan, and only for older 802.11b.

## Convert a frequency

An interactive calculator is on the web page: https://apps.schimpf.es/wifi-manager-and-test-tool/wifi-channel-and-frequency-chart/

## 2.4 GHz channel chart

| Channel | Center frequency (MHz) |
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

Channels 1 to 11 are allowed in the United States. Channels 1 to 13 are allowed in most of Europe.

## 5 GHz examples

| Channel | Center frequency (MHz) |
|---|---|
| 36 | 5180 |
| 40 | 5200 |
| 44 | 5220 |
| 48 | 5240 |
| 100 | 5500 |
| 149 | 5745 |
| 165 | 5825 |

Some 5 GHz channels (around 52 to 144) share spectrum with radar. Your router may have to move off them, which can cause a short drop in the connection.

## 6 GHz examples

| Channel | Center frequency (MHz) |
|---|---|
| 1 | 5955 |
| 5 | 5975 |
| 37 | 6135 |
| 93 | 6415 |

6 GHz is used by WiFi 6E and WiFi 7 devices.

## Which channel should I use?

- In 2.4 GHz, each channel is 20 MHz wide and the channels sit 5 MHz apart. Neighbors on channels 1 and 3 overlap. The only three channels that do not overlap each other are 1, 6 and 11. Use one of them.
- 5 GHz and 6 GHz have many more non-overlapping channels, so crowding is a smaller problem.
- Pick the channel your neighbors use least. A router set to "auto" usually does this, but not always well.
- A wider channel (40, 80 or 160 MHz) gives more speed but takes more room and meets more interference.
- If a device does not see your 5 GHz network, check that your router uses a channel the device supports.

## Find your channel on Android

The WiFi info screen in WiFi Scanner & Network Tools shows your band, channel and link speed, and the WiFi standard (WiFi 4, 5, 6 or 7) of your current connection. It works out the channel from the frequency Android reports, with the formulas above. Android requires the Location permission to read the network name. The app does not use or store your location.

Combine this with the [WiFi signal strength chart](wifi-signal-strength-chart) to see whether the channel or the signal level is the problem.
