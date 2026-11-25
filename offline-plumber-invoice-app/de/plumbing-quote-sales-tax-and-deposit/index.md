# Angebot: Sales Tax und Anzahlung berechnen (Beispiel)

> Sales Tax nur auf steuerpflichtige Positionen addieren, Anzahlung in % auf die Summe setzen, offenen Betrag finden. Beispiel und Rechner.

- Web: https://apps.schimpf.es/offline-plumber-invoice-app/de/plumbing-quote-sales-tax-and-deposit/
- App: Rechnung & Kostenvoranschlag, https://apps.schimpf.es/offline-plumber-invoice-app/de/index.md
## Die drei Zahlen am Ende eines Angebots

Ein Angebot für Installationsarbeiten endet mit drei Beträgen: Steuer, Gesamtsumme und Anzahlung. Sie hängen in fester Reihenfolge voneinander ab. Die Sales Tax ist die US-Verkaufssteuer, die auf den Preis aufgeschlagen wird.

1. Addieren Sie alle Positionen. Jede Position ist Menge × Einzelpreis, gerundet auf den Cent. Das ist die Zwischensumme.
2. Addieren Sie nur die Positionen, die als steuerpflichtig markiert sind. Multiplizieren Sie diesen Betrag mit dem Steuersatz. Das ist die Steuer.
3. Zwischensumme plus Steuer ist die Gesamtsumme.
4. Multiplizieren Sie die Gesamtsumme mit dem Anzahlungsprozentsatz. Das ist die Anzahlung.
5. Gesamtsumme minus der Betrag, den der Kunde schon gezahlt hat, ist der offene Betrag.

Die Offline Plumber Invoice App folgt genau dieser Reihenfolge. Sie rundet kaufmännisch auf den Cent, aus 223,797 wird also 223,80.

## Rechner

An interactive calculator is on the web page: https://apps.schimpf.es/offline-plumber-invoice-app/de/plumbing-quote-sales-tax-and-deposit/

## Beispiel: neue Leitungen im Bad

Der Auftrag hat diese Positionen:

| Position | Menge | Einzelpreis | Steuerpflichtig | Positionssumme |
|----------|-------|-------------|-----------------|----------------|
| PEX-Rohr, 3/4 Zoll (20 mm) | 100 ft (rund 30 m) | 1,20 $ | ja | 120,00 $ |
| Fittings und Ventile | 1 | 292,00 $ | ja | 292,00 $ |
| Arbeitszeit | 6 Std. | 50,00 $ | nein | 300,00 $ |

- Zwischensumme: 120,00 $ + 292,00 $ + 300,00 $ = 712,00 $
- Steuerpflichtiger Betrag: 120,00 $ + 292,00 $ = 412,00 $
- Steuer bei 8,25 %: 412,00 $ × 0,0825 = 33,99 $
- Gesamtsumme: 712,00 $ + 33,99 $ = 745,99 $
- Anzahlung bei 30 %: 745,99 $ × 0,30 = 223,797 $, gerundet 223,80 $
- Offener Betrag nach der Anzahlung: 745,99 $ − 223,80 $ = 522,19 $

Der Steuersatz ist ein einziger Gesamtsatz, wie er in der örtlichen Satztabelle steht (Bundesstaat plus County plus Stadt). Die App nimmt einen Satz pro Dokument.

## Steuer auf die Positionen, nicht auf die Gesamtsumme

Die Steuer gilt für den steuerpflichtigen Betrag. Im Beispiel ergäbe der volle Betrag von 712,00 $ eine Steuer von 58,74 $, also 24,75 $ zu viel. Ob Arbeitszeit steuerpflichtig ist, hängt vom Bundesstaat und von der Art der Arbeit ab. Manche Staaten besteuern Reparaturarbeit, andere nur Material, und manche behandeln Neubau anders als Reparatur. Suchen Sie die Regel für Ihren Staat auf der Website der Steuerbehörde Ihres Staates (Department of Revenue) oder fragen Sie Ihren Steuerberater, bevor Sie Ihre Positionen anlegen.

In der App hat jede Position ein eigenes Kästchen "steuerpflichtig". Preisbuch-Artikel, die als Arbeit markiert sind, starten als nicht steuerpflichtig, alle anderen als steuerpflichtig. Sie können beides in der Position ändern. Jedes Angebot hat seinen eigenen Steuersatz und Anzahlungsprozentsatz, und ein neues Angebot startet mit den Standardwerten aus Ihrem Firmenprofil.

## Die Anzahlung ist ein Anteil der Gesamtsumme

Der Anzahlungsprozentsatz gilt für die Gesamtsumme inklusive Steuer. 30 % Anzahlung auf 745,99 $ sind 223,80 $. Kassieren Sie sie, bevor Sie bei größeren Aufträgen Material bestellen oder anfangen.

Die Anzahlung hat kein eigenes Dokument. Wenn Sie sie kassieren, erfassen Sie sie als Zahlung auf der Rechnung, mit Datum und Zahlart: bar, Scheck oder andere. Die Rechnung zeigt dann den offenen Betrag. Im Beispiel bleiben nach einer zweiten Zahlung von 200,00 $ per Scheck noch 322,19 $.

## Was die App für Sie prüft

- Ein Angebot lässt sich nicht ohne Positionen oder mit einer Position ohne Preis unterschreiben.
- Steuer und Anzahlung aktualisieren sich beim Tippen.
- Sie können keine Zahlung erfassen, die höher ist als der offene Betrag.
- Sobald der Kunde mit dem Finger unterschreibt, ist das Angebot gesperrt. Ein Tipp macht daraus eine Rechnung, und die Positionen werden übernommen.
- Der Rechnungsstatus wechselt nach der ersten Zahlung auf "Partially paid" und auf "Paid", wenn die Zahlungen die Gesamtsumme decken.

Um zuerst den Preis eines Teils festzulegen, lesen Sie [Aufschlag-Formel und Tabelle für Installationsteile](../plumbing-markup-calculator/).

Die App arbeitet ohne Empfang. Sie können das Angebot im Keller schreiben, dort die Unterschrift holen und das PDF später aus dem Postausgang (Outbox) senden.

Die App rechnet in US-Dollar mit einem Sales-Tax-Satz pro Dokument. Mehrwertsteuer berechnet sie nicht.
