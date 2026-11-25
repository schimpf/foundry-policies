# Der Monarch Anleitung zu Ernte, Boden und Volk ernähren

> So viel Korn braucht dein Volk in Der Monarch, wie Felder und Boden die Ernte bestimmen und was Ernähren bewirkt. Mit Formeln und Rechenbeispielen.

- Web: https://apps.schimpf.es/der-monarch/de/der-monarch-feeding-and-harvest-guide/
- App: Der Monarch, https://apps.schimpf.es/der-monarch/de/index.md
Wie viel Korn du dem Volk gibst und was du anbaust, entscheidet in Der Monarch über die meisten Jahre. Diese Anleitung zeigt die Formeln aus dem Spiel und rechnet die Startsituation durch.

## Wie viel Korn das Volk braucht

Der Bedarf liegt bei 7 Scheffel pro Kopf. Gezählt werden Leibeigene, Händler, Klerus und Adel.

**Bedarf = Untertanen × 7**

Zum Start hast du 2.140 Untertanen, der Bedarf beträgt also 2.140 × 7 = 14.980 Scheffel. Im Lager liegen 18.000.

Der Bildschirm Volk ernähren hat einen Schieberegler und Schnellwahlen für 80 %, den Bedarf und 125 %. Korn, das du für die Ernährung zurücklegst, kannst du nicht verkaufen.

## Was das Ernähren mit der Bevölkerung macht

Sei Verhältnis = verfüttertes Korn / Bedarf. Das Spiel sagt die Veränderung pro Jahr so voraus:

- **Geburten:** Leibeigene × 3 % × Verhältnis, das Verhältnis zählt höchstens bis 1,2
- **Todesfälle:** Untertanen × 1,5 %
- **Verhungert:** Liegt das Verhältnis unter 1, sind es Untertanen × (1 − Verhältnis) × 25 %
- **Wanderung:** (Verhältnis, höchstens 1,5, − 1) × Untertanen × 8 %, plus (30 − Steuerdruck) × Untertanen × 0,15 %, plus die Stimmung der Justiz × Untertanen

Der Steuerdruck ist (Zoll + Einkommensteuer) / 2. Die Stimmung der Justiz ist +0,01 bei Milde, 0 bei Gerecht, −0,01 bei Streng und −0,03 bei Grausam. Ein positives Ergebnis bei der Wanderung sind Zuwanderer, ein negatives sind Menschen, die fortziehen.

### Rechenbeispiel: drei Stufen beim Ernähren

Startsituation: 1.820 Leibeigene, 2.140 Untertanen, Zoll 20 %, Einkommensteuer 25 %, Justiz Gerecht. Der Steuerdruck ist 22,5, der Steueranteil an der Wanderung also 7,5 × 2.140 × 0,0015 = 24.

| Verfüttert | Verhältnis | Geburten | Todesfälle | Verhungert | Wanderung | Veränderung gesamt |
|---|---|---|---|---|---|---|
| 80 % (11.984) | 0,8 | 44 | 32 | 107 | −10 | **−105** |
| 100 % (14.980) | 1,0 | 55 | 32 | 0 | +24 | **+47** |
| 125 % (18.725) | 1,25 | 66 | 32 | 0 | +67 | **+101** |

Für 125 % brauchst du 18.725 Scheffel, mehr als die 18.000 im Lager. Zum Start erreichst du das nur, wenn du Korn zukaufst. Der Schieberegler endet bei dem Korn, das du besitzt. Zum Jahresende ist das verfütterte Korn auf das begrenzt, was nach den Ratten übrig ist, plus die Ernte.

Über 120 % gibt es keine zusätzlichen Geburten mehr, aber die Zuwanderung steigt weiter bis 150 %.

## Was du anbaust

Du verteilst dein Land auf Kartoffeln, Korn und Hafer. Der Rest liegt brach. Jede Frucht wird einmal im Jahr zwischen einem niedrigen und einem hohen Ertrag je Morgen ausgewürfelt.

| Frucht | Ertrag je Morgen | Risiko | Bodenverbrauch |
|---|---|---|---|
| Kartoffeln | 2,6–3,5 | gering | 8 |
| Korn | 1,8–5,2 | hoch | 6 |
| Hafer | 2,5–2,7 | keins | 3 |

Die Bodenkraft liegt zwischen 40 und 100 %. Jeder Ertrag wird mit Boden / 100 multipliziert. Der Schwierigkeitsgrad verschiebt den Wurf: Milde bringt bessere Jahre, Hart schlechtere und mehr Verlust durch Ratten.

### Leibeigene begrenzen deine Felder

Jeder Leibeigene bewirtschaftet höchstens 6 Morgen. Willst du mehr Land bestellen als Leibeigene × 6, werden alle Früchte anteilig gekürzt. Mit 1.820 Leibeigenen schaffst du 10.920 Morgen.

### Rechenbeispiel: der Standardplan

Land 10.000 Morgen, Plan 40 % Kartoffeln, 35 % Korn, 15 % Hafer, 10 % brach, Boden 100 %.

1. Bestellt: 4.000 Kartoffeln, 3.500 Korn, 1.500 Hafer. Zusammen 9.000 Morgen, unter der Grenze von 10.920.
2. Niedrigste Ernte: 4.000 × 2,6 + 3.500 × 1,8 + 1.500 × 2,5 = 10.400 + 6.300 + 3.750 = 20.450 Scheffel
3. Höchste Ernte: 4.000 × 3,5 + 3.500 × 5,2 + 1.500 × 2,7 = 14.000 + 18.200 + 4.050 = 36.250 Scheffel
4. Dein Bedarf liegt bei 14.980, also reicht selbst das schlechteste Jahr für alle, noch vor den Ratten.

Die Ratten fressen dann einen Teil des Korns in deinem Lager, bis zu 5 % bei Milde, 10 % bei Normal und 16 % bei Hart.

## Boden

Jedes Jahr ändert sich der Boden um:

**Brache in % × 0,6 − Σ(Anbau in % × Verbrauch / 100)**, gerundet

Für den Standardplan: Verbrauch = 0,40 × 8 + 0,35 × 6 + 0,15 × 3 = 5,75. Die Brache bringt 10 × 0,6 = 6. Die Änderung ist +0,25, gerundet 0, der Boden bleibt bei 100.

Baust du auf allem Land (0 % Brache) nur Kartoffeln an, sinkt der Boden um 8 Punkte im Jahr. Nach 5 Jahren steht er bei 60, und jeder Ertrag ist um 40 % niedriger. Unter 40 fällt der Boden nie.

## Tipps

- Hafer ist die sichere Frucht. Korn bringt zwischen 1,8 und 5,2 je Morgen.
- Lass etwas Land brach liegen, wenn du hart wirtschaftest. Brache gibt 0,6 Bodenpunkte je Prozent zurück.
- Korn lässt sich auch verkaufen. Eine gute Ernte wird zu Talern für Bauten. Siehe die [Rangvoraussetzungen](der-monarch-rank-requirements).
- Krieg kostet Ernte. Jede Kompanie, die du ausschickst, senkt deine Ernte um 2 %.

## Selbst spielen

Der Monarch ist ein Android-Spiel für ein bis vier Spieler auf einem Gerät. Alle Texte im Spiel sind auf Deutsch. Öffne die Bildschirme Volk ernähren und Felder bestellen, um diese Zahlen auszuprobieren.
