# WiFi Signal Strength Chart (dBm to Signal Quality)

> What WiFi dBm values mean, from -30 to -100 dBm. A chart, a quick lookup tool and what to do when your signal is weak.

- Web: https://apps.schimpf.es/wifi-manager-and-test-tool/wifi-signal-strength-chart/
- App: WiFi Scanner & Network Tools, https://apps.schimpf.es/wifi-manager-and-test-tool/index.md
WiFi signal strength is shown as RSSI in **dBm**. The number is negative, and the closer to zero, the stronger the signal. This page gives a chart, a small lookup tool and a few fixes.

## WiFi signal strength chart

| Signal (dBm) | Quality | Bars (of 4) | What to expect |
|---|---|---|---|
| -55 or higher | Excellent | 4 | Full speed. Video calls and streaming are stable. |
| -56 to -67 | Good | 3 | Reliable for streaming, calls and browsing. |
| -68 to -75 | Fair | 2 | Works, but speed drops and calls may stutter. |
| -76 to -99 | Weak | 1 | Slow pages, drops and long delays. |
| -100 or lower | No signal | 0 | Not usable. |

These bands are the ones used by the app WiFi Scanner & Network Tools. Other tools draw the lines a few dBm apart, so treat them as a guide.

## How to read dBm

- dBm is a logarithmic scale. Every 3 dBm change roughly doubles or halves the power.
- -50 dBm has about 1,000 times more power than -80 dBm. A drop from -55 to -75 is a 100-fold loss.
- A change of 1 or 2 dBm is noise. Signal moves by that much when you turn your body or move the phone.
- The value is what your phone receives from the router. It says nothing about how far your router can hear your phone.

### Worked example

You measure -62 dBm in the living room and -79 dBm in the bedroom.

1. Living room: -62 is between -56 and -67, so Good.
2. Bedroom: -79 is between -76 and -99, so Weak.
3. The difference is 17 dBm, which is about 50 times less power in the bedroom (17 / 10 = 1.7, and 10^1.7 is about 50).

Fix the bedroom first.

## Check a value

An interactive calculator is on the web page: https://apps.schimpf.es/wifi-manager-and-test-tool/wifi-signal-strength-chart/

## What lowers your signal

- **Distance.** Signal falls quickly in the first few meters, then more slowly.
- **Walls.** Brick, concrete and stone cost more than drywall. Metal and mirrors cost the most.
- **Band.** 5 GHz and 6 GHz carry less far than 2.4 GHz and are blocked more by walls.
- **Interference.** Neighbor networks on the same channel, microwave ovens and cordless phones add noise. See the [WiFi channel chart](wifi-channel-and-frequency-chart) to find a quieter channel.
- **Router position.** A router on the floor, in a cabinet or in a corner covers less of the home.

## How to improve a weak signal

1. Move the router to a central, higher spot in the open.
2. Walk to the weak room and watch the number live while you move the router or the phone.
3. Change to a less crowded channel.
4. For 2.4 GHz, use channel 1, 6 or 11 so you do not overlap neighbors more than needed.
5. If one room stays weak, add an access point or a mesh node placed halfway to it, wired if possible.

## Measure it on your phone

The WiFi info screen in WiFi Scanner & Network Tools shows your current signal in dBm with the quality name and four-bar meter from the chart above. It also shows band, channel, link speed and WiFi standard. Android requires the Location permission before an app can read the network name. The app does not use or store your location.

Walk through the home with the screen open and note the value in each room. Everything stays on your phone.

## Signal and speed

A strong signal is needed for speed, but the two are different values. Link speed depends on the WiFi standard, channel width and how many devices share the channel. A -50 dBm signal on a busy channel can still be slow. If the signal is good and the connection is still slow, check the channel and run a ping to see latency.
