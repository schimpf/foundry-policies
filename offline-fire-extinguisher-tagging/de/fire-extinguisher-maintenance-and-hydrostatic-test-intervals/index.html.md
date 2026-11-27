# Feuerlöscher Prüffristen und Druckprüfung im Überblick

> Tabelle der NFPA-10-Fristen für monatliche Prüfung, Wartung, 6-Jahres-Wartung und Druckprüfung bei ABC-, CO2-, Wasser- und Schaumlöschern.

- Web: https://apps.schimpf.es/offline-fire-extinguisher-tagging/de/fire-extinguisher-maintenance-and-hydrostatic-test-intervals/
- App: Feuerlöscher-Prüfprotokoll, https://apps.schimpf.es/offline-fire-extinguisher-tagging/de/index.md
## Fristen nach Löschertyp

NFPA 10, Standard for Portable Fire Extinguishers (Ausgabe 2022), legt fest, wie oft jeder tragbare Feuerlöscher geprüft, gewartet und druckgeprüft werden muss. Die Fristen hängen vom Typ ab. Die Tabelle zeigt die Fristen, die die App verwendet.

| Typ | Monatliche Prüfung | Jährliche Wartung | 6-Jahres-Wartung | Druckprüfung |
|---|---|---|---|---|
| ABC-Pulver | alle 31 Tage | 12 Monate | ja | alle 12 Jahre |
| BC-Pulver | alle 31 Tage | 12 Monate | ja | alle 12 Jahre |
| Clean Agent (Gaslöscher) | alle 31 Tage | 12 Monate | ja | alle 12 Jahre |
| Metallbrandpulver (Klasse D) | alle 31 Tage | 12 Monate | nein | alle 12 Jahre |
| CO2 | alle 31 Tage | 12 Monate | nein | alle 5 Jahre |
| Wasser / Wassernebel | alle 31 Tage | 12 Monate | nein | alle 5 Jahre |
| Schaum (AFFF/FFFP) | alle 31 Tage | 12 Monate | nein | alle 5 Jahre |
| Fettbrand (Klasse K) | alle 31 Tage | 12 Monate | nein | alle 5 Jahre |

Quellen: NFPA 10 (2022), Abschnitt 7.2 für die monatliche Prüfung, Abschnitt 7.3 für die jährliche und die 6-Jahres-Wartung und Abschnitt 8.3 für die Druckprüfung. Die zuständige Behörde kann kürzere Fristen verlangen. In Deutschland gelten dafür meist ASR A2.2 und DIN 14406-4 mit eigenen Fristen. Die App rechnet nach NFPA 10.

## Was jede Frist bedeutet

### Monatlich: alle 31 Tage

Eine kurze Sichtprüfung von Standort, Plombe, Manometer, Zustand und Etikett. Die App zählt 31 Tage ab dem letzten monatlichen Termin.

### Jährlich: 12 Monate

Eine gründlichere Wartung, einschließlich mechanischer Teile, Löschmittel sowie Schlauch und Düse. Die nächste Frist liegt 12 Monate nach dem letzten jährlichen Termin. Die [Checklisten-Seite](../nfpa-10-monthly-annual-inspection-checklist/) nennt jeden Punkt.

### 6-Jahres-Wartung

Gilt für die Typen ABC-Pulver, BC-Pulver und Clean Agent in der Tabelle oben. Das Gerät wird entleert und innen untersucht. Die nächste Frist liegt 6 Jahre nach der letzten 6-Jahres-Wartung. Ist keine erfasst, zählt die App 6 Jahre ab dem Herstellungsdatum.

### Druckprüfung: 5 oder 12 Jahre

Der Behälter wird mit Druck geprüft, ob er noch hält. Die nächste Frist liegt ein Prüfintervall nach der letzten Druckprüfung. Ist keine erfasst, zählt die App ab dem Herstellungsdatum.

## Rechenbeispiel

Ein ABC-Pulverlöscher wurde am 2. März 2016 hergestellt. Erfasst sind nur eine monatliche Prüfung am 10. Januar 2026 und eine jährliche Wartung am 15. Juni 2025.

- **Nächste monatliche Prüfung:** 10. Januar 2026 plus 31 Tage ist der 10. Februar 2026.
- **Nächste jährliche Wartung:** 15. Juni 2025 plus 12 Monate ist der 15. Juni 2026.
- **Nächste 6-Jahres-Wartung:** kein Termin erfasst, also 2. März 2016 plus 6 Jahre gleich 2. März 2022. Das Datum liegt lange zurück, das Gerät ist überfällig.
- **Nächste Druckprüfung:** kein Termin erfasst, also 2. März 2016 plus 12 Jahre gleich 2. März 2028.

Nun ein CO2-Löscher, hergestellt am 20. August 2021, ohne weitere Termine. CO2 hat keine 6-Jahres-Wartung, die Zeile lautet "nicht erforderlich". Die Druckprüfung ist am 20. August 2021 plus 5 Jahre, also am 20. August 2026 fällig.

Die Datumsrechnung nutzt Kalendermonate und Kalenderjahre. Fällt ein Datum auf einen Tag, den der Zielmonat nicht hat, rückt es auf den letzten Tag dieses Monats. 31. August plus 6 Monate ergibt den 28. Februar (oder den 29. im Schaltjahr).

## So kennzeichnet die App den Status

Für jede Frist vergleicht die App das Datum mit heute:

- **Überfällig:** die Frist ist abgelaufen.
- **Bald fällig:** monatliche Prüfungen in 7 Tagen oder weniger, alle anderen Posten in 30 Tagen oder weniger.
- **OK:** alles, was später liegt.
- **Nicht erfasst:** kein Datum, ab dem gezählt werden kann.

Ein Feuerlöscher zeigt seinen schlechtesten Posten. Eine durchgefallene letzte Prüfung steht über "überfällig", danach folgen überfällig, bald fällig und OK. Ein Gerät ohne erfasste Daten erscheint als neu.

## Für ein Gerät berechnen

Auf der [Rechner-Seite](../fire-extinguisher-due-date-calculator/) tragen Sie die Termine eines Feuerlöschers ein und sehen alle vier nächsten Fristen.

## Für einen ganzen Standort

Offline fire extinguisher tagging speichert für jeden Feuerlöscher die letzten Termine für monatliche Prüfung, jährliche Wartung, 6-Jahres-Wartung und Druckprüfung und berechnet die nächsten Fristen nach Typ mit den obigen Regeln. Jedes Gerät, jeder Standort und jeder Kunde zeigt OK, bald fällig oder überfällig. Einmal am Tag erinnert die App mit einer Meldung pro Standort, und das Widget auf dem Startbildschirm zeigt die Zahl der überfälligen und der bald fälligen Geräte und den nächsten Standort. Die App erfasst nur die Termine. Für die 6-Jahres-Wartung und die Druckprüfung gibt es keine Checklisten.
