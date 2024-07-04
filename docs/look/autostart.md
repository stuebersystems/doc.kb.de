# Startoptionen

Folgende Situationen: 

Sie möchten es Ihren Kollegen einfach machen und wollen, dass sich DaVinci Look nach dem Start per Doppelklick automatisch an einer voreingestellten Datei anmeldet? Lesen Sie bitte die Schritte 1 bis 3!

Oder möchten Sie auf einem Display, dass nachts herunterfährt nach dem Neustart am Morgen automatisch das Programm starten lassen und eine bestimmte Ansicht zeigen? Lesen Sie bitte die Schritte 1 bis 4!


## Schritt 1: Die Anmeldung am DaVinci Server hinterlegen

Öffnen Sie DaVinci Look auf dem Arbeitsplatz und wählen `Plan > DaVinci Optionen > Plandatei`. Wählen Sie die Serveranmeldung als Standardeinstellung aus und geben die Anmeldedaten für den gewünschten Account ein.

![`Plan > DaVinci Optionen > Plandatei`](/assets/images/look/autostart01.png)

## Schritt 2: Wählen Sie die Startansicht aus
Welche Ansicht nach dem Öffnen gezeigt werden soll, stellen Sie unter `Plan > DaVinci Optionen > Einstellungen` ein.

![Wählen Sie einen Modus aus!](/assets/images/look/autostart02.png)

![Wählen Sie eine Ansicht aus!](/assets/images/look/autostart03.png)

## Schritt 3: Wählen Sie die Startplandatei aus

Sie müssen noch festlegen mit welche Plandatei nach der Anmeldung am DaVinci Server ausgewählt werden soll. Öffnen Sie bitte den Punkt `Plan > Server verwalten > markieren Ihren DaVinci-Server > Bearbeiten > Plandatei`. Wählen Sie die Option "Immer mit der folgenden Plandatei starten" und wählen die gewünschte Datei aus.

![Öffnen Sie den Punkt `Plan > Server verwalten`!](/assets/images/look/autostart04.png)

![Wählen Sie Ihre Startdatei aus!](/assets/images/look/autostart05.png)

Speichern Sie Ihre Einstellungen und schließen das Programm. Wird es erneut aufgerufen, meldet es sich am Server an, wählt die Datei und öffnet die eingestellt Ansicht.


## Schritt 4: DaVinci Look automatisch bei der Rechneranmeldung mit starten

Sie können für Ihr Windows Betriebssystem auswählen, welche Programme beim Start automatisch mit geöffnet werden sollen. Es ist möglich, dass Sie für diese Einstellungen erhöhte Rechte benötigten. Gehen Sie bitte wie folgt vor:

1. Öffnen Sie den DaVinci Programmordner (Standard wäre `C:\Program Files (x86)\Stueber Systems\daVinci 6`) und erstellen eine Verknüpfung der DAVINCILook.exe.

![Rechtsklick > Senden an > Desktop (Verknüpfung erstellen)](/assets/images/look/autostart06.png)

2. Wechseln Sie auf Ihren Desktop und kopieren die Verknüpfung in Ihre Zwischenablage (Markieren und STRG+C).
3. Drücken Sie zeitgleich die Tasten `Windows `und `R`. Es öffnet sich das Fenster `"Ausführen"`. Tippen sie "shell:startup" ein und klicken auf `OK`!

![Tippen Sie shell:startup ein und bestätigen mit OK!](/assets/images/look/autostart07.png)

4. Es öffnet sich das Verzeichnis `Autostart`, fügen Sie über STRG+V die Verknüpfung ein. Fertig!

Wird der Rechner neu gestartet, öffnet sich das Programm DaVinci Look, meldet sich am DaVinci Server an, startet die gewählte Plandatei und ruft Ihnen Ihre gewünschte Ansicht auf!

