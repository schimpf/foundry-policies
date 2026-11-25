# Rechnung: Fälligkeit und Zahlungsverzug berechnen

> Zahlungsziel festlegen, Fälligkeitsdatum ausrechnen und erkennen, ab wann eine Rechnung überfällig ist, mit Rechenbeispiel und Mahnroutine.

- Web: https://apps.schimpf.es/offline-trades-field-forms/de/invoice-due-date-and-overdue/
- App: Field Forms: Arbeitsberichte, https://apps.schimpf.es/offline-trades-field-forms/de/index.md
"Zahlbar innerhalb von 14 Tagen" klingt eindeutig, bis jemand fragt, wann Tag 14 ist oder ab wann die Rechnung überfällig ist. Diese Seite zeigt, wie man zählt, was überfällig heißt und wie man den Überblick ohne Excel-Tabelle behält.

## Die Formel

- **Fälligkeitsdatum** = Rechnungsdatum + Zahlungsziel (in Tagen).
- **Überfällig** = die Rechnung ist unbezahlt und heute liegt nach dem Fälligkeitsdatum.

Eine Rechnung, die am 17. März fällig ist, ist am 17. März noch pünktlich. Überfällig ist sie ab dem 18. März. Eine bezahlte Rechnung ist nie überfällig, egal wie alt sie ist.

## Rechenbeispiel

Sie stellen am 3. März eine Rechnung mit 14 Tagen Zahlungsziel aus.

1. Start ist der 3. März.
2. Zählen Sie 14 Tage dazu: 3 + 14 = 17, das Fälligkeitsdatum ist also der 17. März.
3. Am 17. März ist die Rechnung offen, aber noch nicht überfällig.
4. Am 18. März ist sie 1 Tag überfällig.
5. Am 25. März ist sie 8 Tage überfällig.

Über das Monatsende zählt man genauso. Bei 30 Tagen Zahlungsziel ab dem 20. Juni ist die Rechnung am 20. Juli fällig. Bei 14 Tagen ab dem 25. Februar in einem Jahr ohne Schalttag ist sie am 11. März fällig.

| Rechnungsdatum | Zahlungsziel | Fällig am | Erster Tag überfällig |
|---|---|---|---|
| 3. März | 14 Tage | 17. März | 18. März |
| 20. Juni | 30 Tage | 20. Juli | 21. Juli |
| 25. Februar (kein Schaltjahr) | 14 Tage | 11. März | 12. März |

## Zahlungsziel wählen

- **Kurze Fristen passen zu kleinen Aufträgen.** Sieben bis vierzehn Tage sind bei Privatkunden üblich.
- **Längere Fristen passen zu Firmenkunden,** die oft eigene Zahlungsläufe haben. Vereinbaren Sie das vor Arbeitsbeginn.
- **Nennen Sie das Zahlungsziel schon im Angebot,** dann hat der Kunde es bei Rechnungseingang bereits akzeptiert.
- **Prüfen Sie die Rechtslage.** Verzug und Verzugszinsen unterscheiden sich je nach Land und danach, ob der Kunde Unternehmer oder Verbraucher ist. In Deutschland regelt § 286 BGB den Verzug. Fragen Sie im Zweifel Ihre Handwerkskammer oder Ihren Steuerberater.

## Eine einfache Routine zum Nachfassen

1. **Schicken Sie die Rechnung am selben Tag** wie die Arbeit, als PDF an die E-Mail-Adresse des Kunden.
2. **Prüfen Sie offene Rechnungen einmal pro Woche.** Ein fester Wochentag hilft.
3. **Am Fälligkeitstag** tun Sie nichts. Die Zahlung ist noch nicht verspätet.
4. **Einen Tag überfällig:** schicken Sie eine kurze, freundliche Zahlungserinnerung mit Rechnungsnummer und Betrag.
5. **Eine Woche überfällig:** rufen Sie den Kunden an.
6. **Markieren Sie die Rechnung als bezahlt,** sobald das Geld da ist, mit Zahlungsdatum.

## Was auf die Rechnung gehört

Schreiben Sie diese Angaben auf jede Rechnung, damit es später nichts zu klären gibt:

- Die Rechnungsnummer und das Rechnungsdatum.
- Das Fälligkeitsdatum, als Datum und nicht nur als "14 Tage".
- Den Rechnungsbetrag, mit der Umsatzsteuer als eigene Zeile.
- Firmenname, Adresse, Telefon, E-Mail und Steuernummer.
- Die Zahlungsart, zum Beispiel Ihre Bankverbindung.

Mit einem konkreten Datum ist klar, ab wann gezählt wird. Wenn der Kunde zuerst ein Angebot unterschreibt, gilt als Rechnungsdatum der Tag, an dem Sie die Rechnung ausstellen.

## Anzahlungen und Rabatte

Eine Anzahlung, die Sie schon erhalten haben, verringert den offenen Betrag. Tragen Sie sie als negative Position in die Rechnung ein, dann zeigt die Summe nur den Rest. Rabatte funktionieren genauso. Wie sich das auf die Steuer auswirkt, steht im Rechenbeispiel auf der Seite zur Rechnungssumme.

## Mit Offline Trades Field Forms nachverfolgen

Die Android-App **Offline Trades Field Forms** rechnet die Daten für Sie.

- Das Zahlungsziel stellen Sie einmal in den Einstellungen ein. Standard sind 14 Tage, und das Fälligkeitsdatum lässt sich pro Rechnung ändern.
- Ein Schalter für bezahlt/unbezahlt speichert das Zahlungsdatum.
- Eine Rechnung zeigt **Overdue** (überfällig), wenn sie unbezahlt ist und das Fälligkeitsdatum überschritten ist. Das Zeichen enthält Text und nicht nur eine Farbe.
- Ein Auftrag zeigt seinen dringendsten Status: überfällig, dann unbezahlt, dann angenommenes Angebot, dann Entwurf.
- Das Widget auf dem Startbildschirm zeigt die Summe der offenen und überfälligen Rechnungen und eine Schaltfläche für einen neuen Auftrag. Bei aktiver App-Sperre sind die Beträge ausgeblendet.
- Rechnungen werden automatisch nummeriert (INV-0001 und so weiter), und ein unterschriebenes Angebot wird mit einem Tipp zur Rechnung.
- Die App funktioniert ohne Empfang und ohne Konto. Die Oberfläche ist auf Englisch.
