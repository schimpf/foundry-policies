# Hypothek Monatsrate berechnen: Formel mit Beispiel

> So berechnest du die Monatsrate einer Hypothek mit festem Zins: Formel, Beispiel mit 200.000 Euro bei 2,60 % über 30 Jahre und ein Rechner zum Testen.

- Web: https://apps.schimpf.es/morgage-calc/de/mortgage-monthly-payment-formula/
- App: Hipoteca: Hypothekenrechner, https://apps.schimpf.es/morgage-calc/de/index.md
Eine Hypothek mit festem Zins hat jeden Monat dieselbe Rate. Sie ergibt sich aus einer Formel, der Annuitätenformel (in Spanien "sistema francés" genannt). Diese Seite erklärt die Formel, rechnet ein Beispiel von Hand und zeigt, wohin das Geld geht.

## Die Formel

**Rate = D × r / (1 − (1 + r)^−n)**

- **D** ist der Darlehensbetrag.
- **r** ist der Monatszins: der Jahreszins (TIN, der Sollzins) geteilt durch 12.
- **n** ist die Zahl der Monatsraten: Jahre × 12.

Bei einem Zins von 0 % funktioniert die Formel nicht (Division durch null). Die Rate ist dann D / n.

## Rechenbeispiel

Darlehen von 200.000 Euro, 2,60 % TIN, 30 Jahre.

1. Monatszins: r = 0,026 / 12 = 0,0021667
2. Zahl der Raten: n = 30 × 12 = 360
3. (1 + r)^−360 = etwa 0,4588
4. 1 − 0,4588 = 0,5412
5. Rate = 200.000 × 0,0021667 / 0,5412 = etwa 800,68 Euro pro Monat

Über die gesamte Laufzeit:

- Insgesamt gezahlt: 360 × 800,68 = etwa 288.245 Euro
- Zinsen insgesamt: etwa 88.245 Euro

## Wohin jede Rate geht

Jeden Monat berechnet die Bank Zinsen auf die Restschuld. Der Rest der Rate senkt die Schuld (Tilgung).

1. Zinsen = Restschuld × r
2. Tilgung = Rate − Zinsen
3. Neue Restschuld = alte Restschuld − Tilgung

Monat 1 des Beispiels:

- Zinsen: 200.000 × 0,0021667 = 433,33 Euro
- Tilgung: 800,68 − 433,33 = etwa 367,35 Euro
- Neue Restschuld: etwa 199.632,65 Euro

Weil die Restschuld sinkt, sinken auch die Zinsen, und von jeder späteren Rate geht mehr in die Tilgung. Die Rate bleibt gleich.

| Monat | Zinsanteil | Tilgungsanteil |
|---|---|---|
| 1 | etwa 54 % | etwa 46 % |
| Letzter | unter 1 % | über 99 % |

## Was die Rate am stärksten verändert

- **Laufzeit.** Eine längere Laufzeit senkt die Rate, erhöht aber die Gesamtzinsen. Bei denselben 2,60 % steigt die Rate bei 20 statt 30 Jahren auf etwa 1.070 Euro, die Gesamtzinsen sinken auf rund 56.700 Euro.
- **Zins.** Im Beispiel steigt die Rate bei 3,60 % statt 2,60 % von etwa 801 auf etwa 909 Euro, rund 14 % mehr.
- **Betrag.** Die Rate ist proportional zum Darlehen. Halbiert sich das Darlehen, halbiert sich die Rate.

## Variable und gemischte Zinsen

Die Formel geht von einem gleichbleibenden Zins aus. Bei einer variablen Hypothek ist der Zins der Euríbor plus ein Aufschlag und wird bei jeder Anpassung neu festgelegt (meist alle 12 Monate). Bei jeder Anpassung berechnet die Bank die Rate mit derselben Formel neu, mit diesen Werten:

- D = die Restschuld
- r = der neue Zins geteilt durch 12
- n = die verbleibenden Monate

Eine variable Rate ist also dieselbe Rechnung mit neuen Werten. Die Rate, die du heute siehst, gilt nur bis zur nächsten Anpassung.

## Was die Formel nicht enthält

- **TIN und TAE.** Die Formel verwendet den TIN, den nominalen Zins. Der TAE (der spanische effektive Jahreszins) enthält auch Gebühren und Pflichtprodukte wie Versicherungen und liegt deshalb meist über dem TIN.
- **Kaufnebenkosten.** Steuern, Notar, Grundbuch und die Anzahlung kommen zum Darlehen hinzu und stecken nicht in der Rate.
- **Rundung.** Banken runden jede Rate auf den Cent. Ein Tilgungsplan deiner Bank kann um wenige Cent von der Handrechnung abweichen.

## Rechner

An interactive calculator is on the web page: https://apps.schimpf.es/morgage-calc/de/mortgage-monthly-payment-formula/

## In der App

Hipoteca wendet diese Formel auf dein eigenes Angebot an. Gib Preis, Ersparnisse, Laufzeit und Zinsart ein und sieh Monatsrate, TIN und TAE, die Aufteilung in Tilgung und Zinsen und das Geld, das du am ersten Tag brauchst. Jahrestabelle und Restschuld-Diagramm zeigen, wie die Schuld sinkt, und den Tilgungsplan kannst du als PDF oder CSV exportieren. Bei variablen und gemischten Krediten testet die App auch, was mit der Rate passiert, wenn der Euríbor steigt.

Die Ergebnisse sind Schätzungen und ersetzen kein Angebot deiner Bank.
