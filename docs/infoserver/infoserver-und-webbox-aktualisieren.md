# DaVinci InfoServer und DaVinci WebBox aktualisieren

Wenn Sie in Ihrem Schulnetzwerk die DaVinci-Module aktualisieren möchten, sind folgende Module zu aktualisieren. Das Aktualisieren von DaVinci und DaVinci Look wird nur zur Vollständigkeit aufgezählt und wird hier nicht weiter beschrieben. 

Auf welchen Rechnern|Was muss aktualisiert werden
---|---
 Auf den Clients| [DaVinci](https://download.stueber.de/bin/de/davinci/v6/davinci6.msi) <br/>[DaVinci Look](https://download.stueber.de/bin/de/davinci/v6/davinci6look.msi) 
 Auf dem oder den Serverrechner <br/>(ggfs. laufen der DaVinci InfoServer und der DaVinci Server auf getrennten Rechnern) |[DaVinci Server](https://download.stueber.de/bin/de/davinci/v6/davinci6server.msi)<br/>[DaVinci InfoServer](https://download.stueber.de/bin/de/davinci/v6/davinci6infoserver.msi)<br/>[WebBox Dateien](https://davinci-webbox.stueber.de/) 

## Den DaVinci Server aktualisieren

Möchten Sie eine neue Version des DaVinci Servers einspielen, gehen Sie wie folgt vor:

1. Stellen Sie sicher, dass die DaVinci Benutzer abgemeldet sind.
2. Führen Sie die Installation mit einem aktuelleren [Installationspaket](https://download.stueber.de/bin/de/davinci/v6/davinci6server.msi) des DaVinci Servers aus. Das Setup ersetzt dabei automatisch Ihre bisherigen DaVinci Server Dateien.

## Den DaVinci InfoServer aktualisieren

Möchten Sie eine neue Version des DaVinci InfoServer einspielen, gehen Sie wie folgt vor:

1. Stoppen Sie Ihren Web-Server.
2. Führen Sie die Installation mit einem aktuelleren [Installationspaket](https://download.stueber.de/bin/de/davinci/v6/davinci6infoserver.msi) des DaVinci INFOSERVERS aus. Das Setup ersetzt dabei automatisch Ihre bisherigen DaVinci InfoServer Dateien.

3. Starten Sie den Web-Server neu.

## Die DaVinci WebBox aktualisieren

Möchten Sie eine neue Version der DaVinci WebBox einspielen, gehen Sie wie folgt vor:

1. Prüfen Sie, welche Version Sie aktuell einsetzen. Rufen Sie Ihre WebBox-Seite auf und schauen unten rechts unter dem i-Symbol.

![Klicken Sie auf das i-Symbol!](/assets/images/infoserver/webbox01.png)

![Die eingesetzte Version wird gezeigt.](/assets/images/infoserver/webbox02.png)

Ob eine neuere Ausgabe der WebBox-Dateien vorliegt, können Sie unter [https://davinci-webbox.stueber.de/](https://davinci-webbox.stueber.de/)prüfen.

Laden Sie gegebenenfalls das zip-Archiv mit den WebBox-Dateien auf den Rechner auf dem Ihr Webserver läuft und entpacken die Dateien in das entsprechende Verzeichnis. Die bereits vorhandenen Dateien können vorher gelöscht oder mit dem Inhalt des Zip-Archivs überschrieben werden.

Webserver|Standardverzeichnis für die WebBox-Dateien
---|---
Apache|`c:\xampp\htdocs`
InternetInformationServer|`C:\inetpub\wwwroot`

3. Starten Sie bitte abschließend den Web-Server und Ihren DaVinci-Server neu.