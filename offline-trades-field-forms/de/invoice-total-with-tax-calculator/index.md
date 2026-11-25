# Rechnungssumme mit MwSt. berechnen: Formel und Rechner

> So berechnen Sie Zwischensumme, Umsatzsteuer und Gesamtbetrag einer Rechnung, mit Rechenbeispiel, Rundungsregeln und einem kleinen Rechner.

- Web: https://apps.schimpf.es/offline-trades-field-forms/de/invoice-total-with-tax-calculator/
- App: Field Forms: Arbeitsberichte, https://apps.schimpf.es/offline-trades-field-forms/de/index.md
Bei Rechnungen passieren kleine Fehler: Die Steuer wird auf den falschen Betrag gerechnet, ein Rabatt doppelt abgezogen, oder ein Cent Rundungsdifferenz sorgt dafür, dass die Summe nicht zur Rechnung des Kunden passt. Diese Seite zeigt die genauen Schritte, ein Rechenbeispiel und einen Rechner zum direkten Ausprobieren.

## Die Formel

Eine Rechnung mit einem Steuersatz folgt drei Schritten:

1. **Positionssumme** = Menge × Einzelpreis, für jede Position.
2. **Zwischensumme** (netto) = die Summe aller Positionssummen.
3. **Steuer** = Zwischensumme × Steuersatz. **Gesamtbetrag** (brutto) = Zwischensumme + Steuer.

Die Preise auf den Positionen werden ohne Steuer eingegeben. Die Steuer kommt einmal am Ende auf die Zwischensumme. So lässt sich die Rechnung leicht prüfen, mit einem Steuersatz und einem Steuerbetrag.

## Rechenbeispiel

Ein Heizungsbauer berechnet Arbeitszeit, ein Ersatzteil und einen Kulanzrabatt. Der Steuersatz beträgt 19 %.

| Beschreibung | Menge | Einzelpreis | Positionssumme |
|---|---|---|---|
| Arbeitszeit (Std.) | 2,5 | 48,00 | 120,00 |
| Pumpe | 1 | 86,40 | 86,40 |
| Rabatt | 1 | -20,00 | -20,00 |

- Zwischensumme: 120,00 + 86,40 − 20,00 = 186,40
- Steuer bei 19 %: 186,40 × 0,19 = 35,416, gerundet 35,42
- Gesamtbetrag: 186,40 + 35,42 = 221,82

Der Rabatt ist eine Position mit negativem Preis. Weil er in der Zwischensumme steckt, wird die Steuer auf den geminderten Betrag berechnet. Eine bereits geleistete Anzahlung funktioniert genauso: als negative Position eintragen.

## Rechner

An interactive calculator is on the web page: https://apps.schimpf.es/offline-trades-field-forms/de/invoice-total-with-tax-calculator/

## Rundungsregeln

Es gibt keine Bruchteile eines Cents, deshalb wird jeder Schritt auf die kleinste Währungseinheit gerundet. Die App rundet kaufmännisch (half up): Ein Wert, der genau auf der Hälfte einer Einheit endet, wird von null weg gerundet.

- Gerundet wird jede Positionssumme, danach noch einmal die Steuer.
- Beispiel: 1,5 × 3,33 = 4,995, gerundet 5,00.
- Beispiel: Die Steuer auf eine Zwischensumme von 10,03 bei 17,5 % ist 1,75525, gerundet 1,76.

Die App speichert alle Beträge als ganze Cent und nutzt keine Gleitkommazahlen, deshalb kommt jedes Mal dasselbe Ergebnis heraus. Die Steuer wird einmal auf die Zwischensumme gerundet und nicht pro Position. So entsteht keine Abweichung zwischen den Positionen und dem Gesamtbetrag.

Manche Währungen, etwa der japanische Yen, haben keine Untereinheit. Die App liest die Zahl der Nachkommastellen aus dem Währungscode, deshalb werden diese Beträge auf ganze Einheiten gerundet.

## Häufige Fehler

- **Steuer auf Steuer.** Schlagen Sie keine Steuer auf Preise auf, die schon brutto sind. Geben Sie Nettopreise ein und lassen Sie den Gesamtbetrag die Steuer ergänzen.
- **Rabatt nach der Steuer.** Wenn Sie den Rabatt vom Gesamtbetrag statt von der Zwischensumme abziehen, zahlt der Kunde Steuer auf den Rabatt.
- **Gemischte Steuersätze.** Wird ein Teil des Auftrags mit einem anderen Satz besteuert, teilen Sie ihn auf zwei Rechnungen auf oder fragen Sie Ihren Steuerberater, wie Sie das ausweisen. Die App nutzt einen Steuersatz pro Dokument.
- **Menge in Minuten.** Geben Sie Stunden als Dezimalzahl ein: 90 Minuten sind 1,5, 20 Minuten sind 0,333.

## Welcher Steuersatz gilt

Der Satz hängt davon ab, wo Sie arbeiten und was Sie verkaufen. Fragen Sie Ihr Finanzamt oder Ihren Steuerberater. Diese Seite nennt keinen Steuersatz für ein bestimmtes Land. Die 19 % oben sind nur ein Beispiel.

## Vor Ort mit Offline Trades Field Forms

In der Android-App **Offline Trades Field Forms** legen Sie Positionen mit Beschreibung, Menge und Einzelpreis an. Die App rechnet die Beträge wie oben, ergänzt die Steuer mit dem Satz, den Sie einmal in den Einstellungen festlegen, und nummeriert das Dokument automatisch (INV-0001, INV-0002 und so weiter, mit einem Präfix, das Sie ändern können).

- Legen Sie einmal einen Standard-Steuersatz fest und ändern Sie ihn bei Bedarf pro Dokument.
- Rabatte und Anzahlungen tragen Sie als negative Positionen ein.
- Angebote werden mit einem Tipp zur Rechnung, nachdem der Kunde auf dem Display unterschrieben hat.
- Rechnungen bekommen ein Fälligkeitsdatum, einen Schalter für bezahlt und eine Markierung bei Überfälligkeit.
- Alles funktioniert offline, und die Rechnung verlässt Ihr Handy als PDF über das Teilen-Menü.
- Die Oberfläche der App ist auf Englisch.
