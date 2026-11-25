# Android-Wecker klingelt nicht: Ursachen und Lösungen

> Warum der Android-Wecker nicht klingelt oder zu spät kommt, und eine Checkliste von exakten Alarmen bis zur Akku-Optimierung.

- Web: https://apps.schimpf.es/alarm-clock/de/alarm-not-going-off-android/
- App: Wecker: Aufwach-Aufgaben, https://apps.schimpf.es/alarm-clock/de/index.md
Ein Wecker, der nicht klingelt, wird meist von einer Einstellung blockiert. Diese Seite listet die häufigsten Ursachen unter Android auf und zeigt, wie du jede prüfst.

## Kurze Checkliste

1. Der Wecker ist eingeschaltet und die richtigen Wochentage sind gewählt.
2. Die Uhrzeit stimmt (prüfe morgens und abends, zum Beispiel 6:30 und 18:30 Uhr).
3. Die Weckerlautstärke ist hoch (nicht die Medienlautstärke).
4. Benachrichtigungen für die Wecker-App sind erlaubt.
5. Die Berechtigung für exakte Alarme ist erteilt, falls deine Android-Version danach fragt.
6. Die Akku-Optimierung schränkt die App nicht ein.
7. Die Hintergrundlimits deines Handyherstellers stoppen die App nicht.
8. Du hast den Wecker mit einer Testzeit eine Minute später ausprobiert.

## Ursache 1: Die Weckerlautstärke ist niedrig

Android hat getrennte Lautstärken für Medien, Klingelton und Wecker. Wer die Medienlautstärke senkt, ändert die Weckerlautstärke nicht. Öffne die Lautstärkeanzeige, klappe sie auf und prüfe den Regler für den Wecker. Wecker spielt über den Wecker-Kanal und klingelt daher auch im Lautlos-Modus. Außerdem steigt die Lautstärke langsam an, über eine Zeit von 0 bis 120 Sekunden, die du einstellst (Standard: 30). Bei einem langen Anstieg sind die ersten Sekunden absichtlich leise. Stelle 0 ein, um mit voller Lautstärke zu starten.

## Ursache 2: Berechtigung für exakte Alarme

Android 12 und 12L (API 31 und 32) können Apps das Setzen exakter Alarme verbieten, bis du es erlaubst. Android 13 und neuer erteilen die Berechtigung automatisch an Apps, die Wecker sind. Siehe *Schedule alarms* in der Android-Entwicklerdokumentation. Auf Android 12 oder 12L öffnest du die Spezialzugriffe der App und erlaubst Alarme und Erinnerungen.

## Ursache 3: Benachrichtigungen sind aus

Sind Benachrichtigungen blockiert, erscheint der Weckbildschirm unter Umständen nicht. Öffne die Benachrichtigungseinstellungen der App und schalte sie ein. Ab Android 13 muss die App außerdem die Benachrichtigungsberechtigung abfragen.

## Ursache 4: Vollbild-Hinweise

Ab Android 14 braucht eine App die Berechtigung für Vollbild-Benachrichtigungen, um den Weckbildschirm über dem Sperrbildschirm anzuzeigen. Wecker-Apps erfüllen die Voraussetzung. Prüfe die Berechtigung in den App-Einstellungen, wenn der Bildschirm beim Klingeln dunkel bleibt.

## Ursache 5: Akku-Optimierung

Android spart Strom, indem es Apps im Hintergrund einschränkt. Nimmst du deine Wecker-App von der Akku-Optimierung aus, sinkt das Risiko, dass das System sie verzögert oder beendet. Öffne die Akkueinstellungen der App und wähle die Option ohne Einschränkung.

## Ursache 6: Akku-Sparfunktionen der Hersteller

Manche Hersteller setzen eigene Limits auf Android obendrauf. Xiaomi, Redmi, Poco, Samsung, Huawei, Honor, OnePlus, Oppo, Vivo und Realme sind die üblichen. Sie beenden Apps, die du aus der Übersicht wischst, oder schicken sie schlafen. Die Community-Seite *Don't kill my app* (dontkillmyapp.com) dokumentiert, was jeder Hersteller tut. Die Einrichtungshilfe von Wecker enthält Schritte für diese Marken.

## Ursache 7: Neustart und Zeitänderungen

Ein Wecker muss nach einem Neustart, nach einer Zeitänderung und nach einem Zeitzonenwechsel neu gestellt werden. Wecker erledigt das selbst. Bei einer anderen App öffnest du sie nach einem Update oder Neustart einmal und prüfst, ob der nächste Wecker noch angezeigt wird.

## Wecker testen

Warte nicht bis morgen. Stelle einen Testwecker eine Minute später und sperre den Bildschirm. Klingelt er und geht der Bildschirm an, funktionieren die Einstellungen.

## So hilft Wecker

- Eine Einrichtungshilfe beim ersten Start führt durch die Einstellungen für exakte Alarme, Benachrichtigungen, Vollbild und Akku und zeigt markenspezifische Schritte.
- Ein Selbsttest-Wecker klingelt eine Minute später.
- Die Einrichtungshilfe kannst du jederzeit in den Einstellungen erneut öffnen.
- Der Wecker wird über die Wecker-Schnittstelle des Systems gestellt, die Android als sichtbaren Wecker des Nutzers behandelt.
- Verschiebst oder löschst du deine eigene Tondatei, spielt stattdessen ein mitgelieferter Ton statt Stille.
- Verlässt du eine Aufwach-Aufgabe, klingelt der Wecker nach einer Minute erneut, und auch nach einem Neustart, wenn er gerade geklingelt hat.

Wecker hat keine Internetberechtigung, kein Konto und keine Analyse. Die App ist Open Source unter der GNU GPL v3 oder neuer. Öffne die App, schließe die Einrichtungshilfe einmal ab und starte den Selbsttest.
