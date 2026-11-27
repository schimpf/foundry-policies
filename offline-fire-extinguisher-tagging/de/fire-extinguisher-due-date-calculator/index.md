# Feuerlöscher Prüffristen berechnen (NFPA 10)

> Löschertyp und letzte Termine eingeben und die nächsten Fristen für monatliche Prüfung, Wartung, 6-Jahres-Wartung und Druckprüfung berechnen.

- Web: https://apps.schimpf.es/offline-fire-extinguisher-tagging/de/fire-extinguisher-due-date-calculator/
- App: Feuerlöscher-Prüfprotokoll, https://apps.schimpf.es/offline-fire-extinguisher-tagging/de/index.md
## Nächste Fristen berechnen

Wählen Sie den Löschertyp und tragen Sie die Termine ein, die Sie haben. Lassen Sie ein Feld leer, wenn es keinen Nachweis gibt. Der Rechner nutzt dieselben Regeln wie die App und folgt NFPA 10, Standard for Portable Fire Extinguishers (Ausgabe 2022).

An interactive calculator is on the web page: https://apps.schimpf.es/offline-fire-extinguisher-tagging/de/fire-extinguisher-due-date-calculator/

## Die Formeln

Jede nächste Frist beginnt beim zuletzt dokumentierten Termin.

| Posten | Nächste Frist | Ersatzweise Herstellungsdatum? |
|---|---|---|
| Monatlich | letzte monatliche Prüfung + 31 Tage | nein |
| Jährlich | letzte jährliche Wartung + 12 Monate | nein |
| 6-Jahres-Wartung | letzte 6-Jahres-Wartung + 6 Jahre | ja |
| Druckprüfung | letzte Druckprüfung + 5 oder 12 Jahre | ja |

- Die 6-Jahres-Wartung gilt für ABC-Pulverlöscher, BC-Pulverlöscher und Clean-Agent-Löscher (Gaslöscher). Bei den anderen Typen steht in der Zeile "nicht erforderlich".
- Das Intervall der Druckprüfung beträgt 12 Jahre für ABC, BC, Clean Agent und Metallbrandpulver (Klasse D) und 5 Jahre für CO2, Wasser, Schaum und Fettbrandlöscher (Klasse K, Nasschemikalie).
- Für die monatliche und die jährliche Frist gibt es keinen Ersatz. Fehlt der letzte monatliche oder jährliche Termin, lautet das Ergebnis "nicht erfasst".

Die vollständige Liste nach Typ steht in der [Fristentabelle](../fire-extinguisher-maintenance-and-hydrostatic-test-intervals/).

## So wird der Status bestimmt

Der Rechner zählt die Tage zwischen heute und der Frist.

- **Überfällig:** weniger als 0 Tage übrig.
- **Bald fällig:** 0 bis 7 Tage bei der monatlichen Prüfung, 0 bis 30 Tage bei den anderen Posten.
- **OK:** mehr Tage als das.

## Rechenbeispiel

Ein Wasserlöscher wurde am 14. Mai 2019 hergestellt. Die letzte monatliche Prüfung war am 1. November 2026, die letzte jährliche Wartung am 20. Dezember 2025, eine Druckprüfung ist nicht dokumentiert. Heute ist der 27. November 2026.

1. **Monatlich:** 1. November 2026 + 31 Tage = 2. Dezember 2026. Das sind 5 Tage, also bald fällig (7 Tage oder weniger).
2. **Jährlich:** 20. Dezember 2025 + 12 Monate = 20. Dezember 2026. Das sind 23 Tage, also bald fällig (30 Tage oder weniger).
3. **6 Jahre:** Wasserlöscher brauchen sie nicht, also nicht erforderlich.
4. **Druckprüfung:** kein Datum erfasst, also 14. Mai 2019 + 5 Jahre = 14. Mai 2024. Das liegt in der Vergangenheit, der Löscher ist 927 Tage überfällig.

Der Löscher erscheint als überfällig, ausgelöst durch die Druckprüfung, weil "überfällig" vor "bald fällig" steht.

## Sonderfälle

- **Monatsende:** 31. August + 6 Monate ergibt den letzten Tag des Zielmonats, den 28. Februar oder in einem Schaltjahr den 29. Der 29. Februar + 1 Jahr ergibt den 28. Februar.
- **Durchgefallene Prüfung:** In der App steht ein Gerät mit durchgefallener letzter Prüfung im Status über "überfällig". Der Rechner hier zeigt nur Termine.
- **Strengere Vorgaben vor Ort:** Die zuständige Behörde kann kürzere Fristen verlangen. Dann gilt die kürzere Frist. In Deutschland gelten dafür meist ASR A2.2 und DIN 14406-4, die eigene Fristen haben. Die App rechnet nach NFPA 10.

## Für einen ganzen Standort

Termine in einen Rechner zu tippen reicht für ein Gerät. Bei einem Standort mit 40 Feuerlöschern speichert Offline fire extinguisher tagging die Termine auf dem Handy, berechnet jede nächste Frist nach Typ mit diesen Formeln und zeigt überfällige Geräte zuerst. Sie scannen den QR-Code oder Barcode am Etikett, um ein Gerät zu öffnen. Die App funktioniert ohne Empfang und braucht kein Konto. Die Gratisversion fasst 25 Feuerlöscher, ein Standort mit 40 braucht Pro.

Die [NFPA-10-Checkliste](../nfpa-10-monthly-annual-inspection-checklist/) behandelt die monatlichen und jährlichen Prüfungen, die diese Termine aktualisieren.
