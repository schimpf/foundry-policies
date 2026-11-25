# Tonleiter-Intervalle: Moll, Phrygisch, Harmonisch Moll

> Halbtonschritte für Moll, Dur, Phrygisch, Harmonisch Moll und Moll-Pentatonik, plus das Frequenzverhältnis jedes Halbtons beim Transponieren.

- Web: https://apps.schimpf.es/tekkno-rave-daw/de/scale-intervals-chart/
- App: Tekkno Rave DAW: Beat-Maker, https://apps.schimpf.es/tekkno-rave-daw/de/index.md
Dunkle Hardtechno-Leads und Acid-Stabs liegen meist in Moll oder Phrygisch. Diese Seite listet die Halbtonschritte von fünf gängigen Tonleitern auf, zeigt, wie du sie von jedem Grundton aus bildest, und nennt das Frequenzverhältnis jedes Halbtons, damit du siehst, was beim Transponieren eines Samples passiert.

## Tabelle der Tonleiter-Intervalle

Die Zahlen sind Halbtöne über dem Grundton. Der Grundton ist 0, die Oktave ist 12.

| Tonleiter | Halbtöne ab dem Grundton | Töne |
|-----------|--------------------------|------|
| Moll (natürliches Moll) | 0, 2, 3, 5, 7, 8, 10 | 7 |
| Dur | 0, 2, 4, 5, 7, 9, 11 | 7 |
| Phrygisch | 0, 1, 3, 5, 7, 8, 10 | 7 |
| Harmonisch Moll | 0, 2, 3, 5, 7, 8, 11 | 7 |
| Moll-Pentatonik | 0, 3, 5, 7, 10 | 5 |

Diese Intervallfolgen gehören zur gängigen westlichen Musiktheorie. Eine ausführliche Darstellung findest du bei Kostka und Payne, *Tonal Harmony* (McGraw-Hill, 8. Auflage, 2017).

## Wie klingt welche Tonleiter?

- Moll hat eine kleine Terz (3 Halbtöne). Sie gibt den dunklen, ernsten Klang, der im Techno häufig ist.
- Phrygisch ist Moll mit kleiner Sekunde (1 Halbton). Der enge Schritt über dem Grundton ergibt den angespannten, aggressiven Sound vieler Hardcore- und Gabber-Leads.
- Harmonisch Moll ist Moll mit erhöhter Septime (11 Halbtöne). Der große Abstand zwischen dem 6. und 7. Ton gibt einen dramatischen, orientalisch klingenden Schub.
- Dur klingt heller und kommt in harten Stilen seltener vor, passt aber zu euphorischen Hardcore-Melodien.
- Moll-Pentatonik lässt den 2. und 6. Ton weg. Mit nur fünf Tönen klingt fast nichts falsch, deshalb eignet sie sich für Riffs.

## So bildest du eine Tonleiter von jedem Grundton

1. Nummeriere die 12 Töne ab dem Grundton: C = 0, Cis = 1, D = 2, Dis = 3, E = 4, F = 5, Fis = 6, G = 7, Gis = 8, A = 9, B = 10, H = 11.
2. Addiere die Nummer des Grundtons zu jedem Intervall aus der Tabelle.
3. Ist die Summe 12 oder größer, ziehe 12 ab.
4. Wandle die Zahlen zurück in Tonnamen.

Im deutschen Notennamen-System heißt der Ton 10 B (in der englischen Schreibweise A sharp oder B flat) und der Ton 11 H.

### Rechenbeispiel: F-Phrygisch

F ist 5. Phrygisch ist 0, 1, 3, 5, 7, 8, 10.

- 5 + 0 = 5, F
- 5 + 1 = 6, Fis (Ges)
- 5 + 3 = 8, Gis (As)
- 5 + 5 = 10, B
- 5 + 7 = 12, das ist 0, C
- 5 + 8 = 13, das ist 1, Cis (Des)
- 5 + 10 = 15, das ist 3, Dis (Es)

F-Phrygisch besteht aus F, Ges, As, B, C, Des, Es.

## Frequenzverhältnis jedes Halbtons

Ein Sample per Resampling zu transponieren ändert seine Abspielgeschwindigkeit. In der gleichstufigen Stimmung mit 12 Tönen multipliziert jeder Halbton die Frequenz mit der zwölften Wurzel aus 2:

Verhältnis = 2^(Halbtöne / 12)

| Halbtöne | Verhältnis |
|----------|------------|
| 0 | 1,0000 |
| 1 | 1,0595 |
| 2 | 1,1225 |
| 3 | 1,1892 |
| 4 | 1,2599 |
| 5 | 1,3348 |
| 6 | 1,4142 |
| 7 | 1,4983 |
| 8 | 1,5874 |
| 9 | 1,6818 |
| 10 | 1,7818 |
| 11 | 1,8877 |
| 12 | 2,0000 |

Negative Werte gehen nach unten: -12 Halbtöne ergeben ein Verhältnis von 0,5, also halbe Geschwindigkeit und eine Oktave tiefer. Resampling ändert auch die Länge des Samples. Ein Sample, das mit dem Verhältnis 2 gespielt wird, dauert nur halb so lang.

## Rechenbeispiel: eine Rasterzeile in A-Moll

Tekkno Rave DAW ordnet Rasterzeilen mit dieser Regel einer Tonhöhe zu. Zeile 0 ist die unterste Zeile, und eine höhere Zeile ist ein höherer Ton. Bei eingeschaltetem Einrasten auf die Tonleiter ist jede Zeile die nächste Stufe der Tonleiter, also liegt jede Zeile in der Tonart. Samples sind auf C3 gestimmt, das ist MIDI-Note 48, und Halbton 0 bedeutet C3.

Für eine Tonleiter mit n Tönen gilt:

Halbtöne = Grundton + 12 x Oktavverschiebung + 12 x (Zeile div n) + Intervall[Zeile mod n]

Nimm A-Moll (Grundton 9, 7 Töne), Oktavverschiebung 0 und Zeile 9:

1. 9 div 7 = 1, das Pattern ist also eine Oktave nach oben gelaufen: 12 x 1 = 12.
2. 9 mod 7 = 2, und das dritte Intervall von Moll (Index 2) ist 3.
3. Summe = 9 + 0 + 12 + 3 = 24 Halbtöne.
4. Verhältnis = 2^(24 / 12) = 4,0.
5. Der Ton ist MIDI 48 + 24 = 72, das ist C5.

Zur Kontrolle zähle die A-Moll-Stufen ab Zeile 0 nach oben: A, H, C, D, E, F, G, A, H, C. Zeile 9 ist der zehnte Ton, also C. Das passt.

Bei ausgeschaltetem Einrasten sind die Zeilen einfache Halbtöne (Halbtöne = Grundton + 12 x Oktavverschiebung + Zeile), und Zeilen in der Tonleiter werden nur eingefärbt.

## In der App ausprobieren

Tekkno Rave DAW hat ein Pattern-Raster mit 12 Zeilen, 8, 16, 32 oder 64 Schritten und einer Oktavverschiebung von -2 bis +2. Wähle Moll, Dur, Phrygisch, Harmonisch Moll oder Moll-Pentatonik mit beliebigem Grundton, schalte das Einrasten ein, und jede Zeile bleibt in der Tonart. Öffne ein Pattern und male Noten, um die Tonleitern aus dieser Tabelle zu hören.
