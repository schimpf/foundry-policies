# Nagios und Icinga: Soft State und Hard State erklärt

> Was Soft State und Hard State in Nagios und Icinga 2 bedeuten, wie Prüfversuche zählen und wie lange ein Ausfall bis zum Hard State braucht.

- Web: https://apps.schimpf.es/tinag2/de/nagios-soft-vs-hard-states-explained/
- App: Tinag2: Icinga & Nagios Alarme, https://apps.schimpf.es/tinag2/de/index.md
Ein Service in Nagios, Naemon oder Icinga 2 alarmiert nicht beim ersten fehlgeschlagenen Check. Er durchläuft zuerst einen Soft State und wird erst nach mehreren fehlgeschlagenen Checks in Folge zum Hard State. Diese Seite erklärt die Zustände, den Versuchszähler und das Timing an einem durchgerechneten Beispiel.

## Die vier Service-Zustände

Jedes Check-Plugin endet mit einem Exit-Code. Der Monitoring-Kern macht daraus einen Zustand. Das folgt den Nagios Plugin Development Guidelines (nagios-plugins.org) und der Icinga-2-Dokumentation, Kapitel "Monitoring Basics".

| Exit-Code | Zustand | Bedeutung |
|---|---|---|
| 0 | OK | Der Check war erfolgreich. |
| 1 | WARNING | Der Wert liegt außerhalb der Warnschwelle. |
| 2 | CRITICAL | Der Wert liegt außerhalb der kritischen Schwelle, oder der Service fällt aus. |
| 3 | UNKNOWN | Das Plugin konnte nicht entscheiden, zum Beispiel wegen eines falschen Arguments oder eines Timeouts. |

Bei Hosts ist es einfacher. Ein Host ist UP oder DOWN. Thruk meldet außerdem UNREACHABLE: ein Host, der nicht erreichbar ist, weil etwas zwischen Monitoring-Server und Host ausgefallen ist.

## Soft und Hard als Zustandstyp

Der Zustandstyp sagt, wie sicher sich der Kern über das Problem ist.

- **Soft**: Ein Check ist fehlgeschlagen, aber die Zahl der fehlgeschlagenen Checks liegt noch unter `max_check_attempts`. Der Kern prüft weiter, jetzt im kürzeren Retry-Intervall.
- **Hard**: Die fehlgeschlagenen Checks haben `max_check_attempts` erreicht, oder der Zustand wechselte von einem harten Problemzustand in einen anderen. Ab hier werden normalerweise Benachrichtigungen verschickt.

Ein Soft State, der vor dem letzten Versuch wieder auf OK geht, wird nie zum Hard State. Das filtert kurze Aussetzer heraus, etwa ein verlorenes Paket.

## Die drei Einstellungen, die das Timing bestimmen

Jeder Host und jeder Service hat diese Einstellungen in der Konfiguration:

1. `check_interval`: Zeit zwischen den Checks, solange der Zustand stabil ist.
2. `retry_interval`: Zeit zwischen den Checks, solange der Zustand soft ist.
3. `max_check_attempts`: Wie viele fehlgeschlagene Checks in Folge den Zustand hart machen. Der erste fehlgeschlagene Check zählt als Versuch 1.

## Wie lange es bis zum Hard State dauert

Gerechnet ab dem ersten fehlgeschlagenen Check:

Zeit bis hard = (`max_check_attempts` − 1) × `retry_interval`

Gerechnet ab dem Moment, in dem der Service wirklich ausfiel, kommt im schlechtesten Fall ein volles Check-Intervall dazu, weil der Ausfall direkt nach einem erfolgreichen Check beginnen kann:

schlechtester Fall = `check_interval` + (`max_check_attempts` − 1) × `retry_interval`

## Durchgerechnetes Beispiel

Einstellungen: `check_interval` 5 Minuten, `retry_interval` 1 Minute, `max_check_attempts` 3.

1. 09:55:00 Uhr. Der Check ist erfolgreich. Zustand OK.
2. 09:55:30 Uhr. Der Service fällt aus. Noch merkt es niemand.
3. 10:00:00 Uhr. Der Check schlägt fehl. Zustand CRITICAL, soft, Versuch 1/3.
4. 10:01:00 Uhr. Der Check schlägt fehl. CRITICAL, soft, Versuch 2/3.
5. 10:02:00 Uhr. Der Check schlägt fehl. CRITICAL, hard, Versuch 3/3. Die Benachrichtigungen beginnen.

Der Zustand wurde 2 Minuten nach dem ersten fehlgeschlagenen Check hart: (3 − 1) × 1 Minute. Er wurde 6,5 Minuten nach dem tatsächlichen Ausfall hart. Der schlechteste Fall für diese Einstellungen ist 5 + 2 = 7 Minuten.

```
schlechtester Fall: 5 Min. (Check-Intervall) + 2 x 1 Min. (Retries) = 7 Min.
                    |#####|##|
```

Wäre der Check um 10:01:00 Uhr erfolgreich gewesen, wäre der Service wieder auf OK gegangen, ohne je hart zu werden, und niemand wäre benachrichtigt worden.

## Die Zahlen anpassen

- Ein höheres `max_check_attempts` entfernt mehr Fehlalarme, verzögert aber echte Alarme.
- Ein kürzeres `retry_interval` bringt den Hard State früher, ohne mehr Rauschen im Takt des stabilen Zustands.
- Für einen sehr wichtigen Service hält ein niedriges `max_check_attempts` wie 2 zusammen mit einem kurzen Retry-Intervall die Verzögerung klein.

## Ein Detail bei Icinga 2

Icinga 2 setzt seinen internen Zähler `check_attempt` auf 1 zurück, sobald ein Zustand hart wird. Liest du bei einem harten Problem den rohen API-Wert, kann dort 1/3 statt 3/3 stehen. Tinag2 zeigt harte Probleme wie Nagios als max/max.

## Soft und Hard in Tinag2

Tinag2 ist ein Android-Client für Icinga 2 und für Nagios/Naemon über Thruk. Die App liest Zustandstyp und Versuchszähler vom Server und nutzt sie an drei Stellen:

- **Problem-Detail** zeigt Zustandstyp und Versuche, zum Beispiel "soft 2/3" oder "hard 3/3".
- **Hard only** ist ein Filter auf dem Problems-Bildschirm und blendet Soft-Probleme aus.
- **Alarmregeln** überspringen Soft States standardmäßig, du wirst also nur bei harten Problemen benachrichtigt. Das kannst du auf dem Alerts-Bildschirm abschalten. Außerdem gibt es die Option, 5 Minuten vor dem Alarm zu warten, gemessen ab der letzten Zustandsänderung des Problems. Das dämpft Checks, die ständig hin- und herspringen.

Die App fragt den Server alle 15 Minuten im Hintergrund ab sowie beim Herunterziehen zum Aktualisieren. Ein hartes Problem erreicht dein Smartphone daher beim nächsten Abgleich nach dem Wechsel auf hart, nicht sekundengenau.

Tinag2 liest Probleme nur und führt Aktionen darauf aus. Check-Intervalle und Versuchszahlen ändert die App nicht; das machst du in deiner Icinga- oder Nagios-Konfiguration.

Tinag2 lässt dich harte Probleme auf dem Smartphone filtern, durchsuchen und bestätigen und schickt Alarme nur für die Probleme, die für dich zählen. Füge in der App deinen Icinga-2- oder Thruk-Server hinzu, um es auszuprobieren.
