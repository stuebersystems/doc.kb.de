# Silent-Mode und Silent-Setup

## Was ist der Silent-Mode

Mit Silent-Mode benennt STÜBER SYSTEMS den Aufruf der Anwendung durch Parameter zur Durchführung von bestimmten Funktionalitäten, ohne dass ein Programmfenster geöffnet oder eine Programmeingabe vom Benutzer erwartet wird. Alle wichtigen Informationen zur Durchführung werden durch die Parameter bestimmt.

Zweck des Silent-Mode ist es, die Anwendung durch z.B. den Taskmanager von Windows im Hintergrund wiederkehrende Aufgaben erledigen zu lassen, ohne dass sich ein Benutzer darum kümmern müsste, also zur Automatisierung bestimmter Aufgaben.

## MAGELLAN ADMINISTRATOR im Silent-Mode starten

### Übersicht der Silent-Mode Aufgaben

Der Magellan-Administrator erlaubt folgende Aufgaben im Silent-Mode zu erledigen:

*	Datenbank-Anmeldung
*	Benutzerrechte synchronisieren
*	Import über das Magellan-Importformat

Diese Punkte werden ausführlich in den kommenden Punkten erläutert.

### MAGELLAN Datenbank-Anmeldung

Sie haben die Möglichkeit den MAGELLAN ADMIMINISTRATOR direkt ohne Eingabe von Benutzernamen, Passwort und Auswahl der Datenbank zu starten, wenn Sie diese Informationen einfach als Parameter angeben.

Parameter:

| Nr. | Parameter                   |
|-----|-----------------------------|
| 1.  | /Login=Benutzername         |
| 2.  | /Keyword=Passwort           |
| 3.  | /Connection=Datenbank-Alias |

> #### warning::Wichtig!
>
> Jegliche weitere Silent-Mode Funktion hängt von diesen Parametern ab. Das bedeutet diese Parameter sind Pflichtangaben für alle weiteren Silent-Mode Aufgaben.
Die Parameter der Datenbank-Anmeldung sind die einzigen Parameter die mit anderen Silent-Mode Funktionen kombinierbar sind.

## MAGELLAN Benutzerrechte synchronisieren

Eine oft wiederkehrende Aufgabe ist das Synchronisieren der Benutzerrechte. Zusätzlich zu den Parametern der Datenbank-Anmeldung müssen folgende Parameter angegeben werden.

| Nr. | Parameter |
|-----|-----------|
| 1.  | /UserSync |

## Import über das MAGELLAN-Importformat

Der Import von Daten ist größtenteils ein einmaliger Import zum Hinzufügen von Fremddaten nach Magellan. Für Schüler- und Lehrerdaten gibt es aber die Möglichkeit, die Stammdaten zu aktualisieren.
Voraussetzung für eine solche Aktualisierung ist, dass die Fremddaten mit einer externen GUID importiert wurden und die Aktualisierung anhand dieses Feldes Externe GUID (Feld GUIDExtern) zur nachträglichen Wiedererkennung der Datensätze, aktualisiert werden. Zusätzlich zu den Parametern der Datenbank-Anmeldung müssen folgende Parameter angegeben werden.

### Parameter

| Nr. | Parameter |
|-----|-----------|
| 1.  | /UserSync |

Der Dateiname der Importdatei muss der Importspezifikation entsprechen:
* Schüler-Stammdaten: schueler.import.csv
* Lehrer-Stammdaten: lehrer.import.csv

### Beispiel

Den MAGELLAN ADMIMINISTRATOR  im Silent-Mode aufrufen, zum Import von Schüler-Stammdaten mit dem Firebird Standard SYSDBA und Passwort:

```
C:\Programme\Stüber Systems\MagAdmin.exe /Login=SYSDBA 
/Keyword=masterkey 
/Connection=Magellan /Import=“C:\Import\schueler.import.csv“ /Mandant=1
```

> #### warning::Wichtig!
>
> Achten Sie bitte darauf, dass in Windows ein parametrisierter Aufruf nicht länger als 260 Zeichen sein darf.

## Installation per Silent-Setup-Parameter

Grundsätzlich basiert unsere Installation auf der MSI-Technologie. Mit dieser MSI-Technologie wird beispielsweise auch MS Office installiert.

### Silent-Setup für MAGELLAN

msiexec /i "C:\MySetup\Magellan7.msi" /q INSTALLMODE="Server" APPDIR="C:\MyFolder\Magellan"

msiexec /i "C:\MySetup\Magellan7.msi" /q INSTALLMODE="Client" APPDIR="C:\MyFolder\Magellan"

msiexec /x "C:\MySetup\Magellan7.msi" /q

Hinweis 1: /i bedeutet immer Installation und /x immer Deinstallation.

Hinweis 2: Unter Vista müssen diese Kommandozeilenaufrufe mit Administratorenrechten gestartet werden.

### Silentinstallation DAVINCI

Installation: msiexec /i "C:\MySetup\daVinci.msi" /q APPDIR="C:\Stueber Systems\daVinci6"

Deinstallation: msiexec /x "C:\Stueber Systems\daVinci6.msi" /q

Hinweis 1: /i bedeutet immer Installation und /x immer Deinstallation.

Hinweis 2: Unter Vista müssen diese Kommandozeilenaufrufe mit Administratorenrechten gestartet werden.
