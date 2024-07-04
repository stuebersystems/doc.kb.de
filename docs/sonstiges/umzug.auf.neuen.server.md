# Umzug auf einen neuen Server

Für den Fall, dass Sie einen neuen Serverrechner anschaffen, finden Sie nachstehend eine Übersicht, der notwendigen Schritte.

> Bitte aktualisieren Sie vorab auch bitte den alten DaVinci auf die Version, mit der Sie Ihren neuen Server bespielen. Damit stellen Sie sicher, dass Daten, die übertragen werden gleich aktuell sind. 

## Installation des neuen Servers

Unsere Installationspakete finden Sie im  [Downloadbereich](https://davinci.stueber.de/download.php) 

Bitte führen Sie die gewünschten Installation aus, Anleitung dazu finden Sie hier: 

[DaVinci Server](https://doc.davinci6.stueber.de/06.enterprise/01.installation/).
[DaVinci](https://doc.davinci6.stueber.de/00.allgemein/installation/)
[DaVinci Look](https://doc.davinci6.stueber.de/05.look/01.installation/)

Soll der DaVinci InfoServer wieder eingerichtet werden, finden Sie die Anleitung von der Einrichtung des Webservers bis zur WebBox im Abschnitt [Live-Daten im Internet](https://doc.davinci6.stueber.de/09.infoserver/allgemeines/).

## Lizenzierung

Wenn Sie nur den DaVinci Server einrichten möchten, ist keine Lizenz auf dem Serverrechner nötig, die vorausgesetzte Lizenzierung wird über die DaVinci Clients abgefragt. Lediglich wenn Sie den DaVinci InfoServer verwenden, muss unter `Systemsteuerung (klassische Ansicht) > DaVinci Server Control > Unterkarte Dienst > Schaltfläche Lizenz` eine entsprechende Lizenz eingetragen werden.

## Übernahme von Daten des alten Servers

> Bevor Sie Daten auf den neuen Server übertragen, vergewissern Sie sich bitte, dass der "alte" DaVinci Server-Dienst gestoppt wurde! Den Dienst können Sie unter `Systemsteuerung (klassische Ansicht) > DaVinci Server Control > Unterkarte Dienst` stoppen.

### Verzeichnis Arbeitsbereich

Speicherort: `C:\Users\Public\Documents\Stueber Systems\daVinci 6\Arbeitsbereich`

Der Arbeitsbereich enthält die vom DaVinci Server verwalteten Plandateien, mitunter Backup-Dateien und die DaVinci.users-Datei, die die Benutzerverwaltung und die Plandateienstruktur des DaVinci EXPLORERs.

Sollten Sie sich nicht sicher sein, an welcher Stelle sich Ihr Arbeitsbereichverzeichnis befindet, können Sie in dem Control (`Systemsteuerung (klassische Ansicht) > DaVinci Server Control > Unterkarte Dienst`) auch auf der Unterkarte `Arbeitsbereich`nachsehen.

Dieses Verzeichnis legen Sie auf dem neuen Rechner nach der Installation unter dem Standardpfad ab, währenddessen muss der DaVinci Server Dienst auf dem neuen Server gestoppt werden. Starten Sie ihn anschließend bitte wieder.

### weitere Verzeichnisses

Speicherorte: 

* `C:\Users\Public\Documents\Stueber Systems\daVinci 6\...`
* `C:\ProgramData\Stueber Systems\daVinci 6\...`
* `C:\Users\Ihr.Benutzer\AppData\Roaming\Stueber Systems\daVinci 6...` Bitte prüfen Sie, ob dieses Verzeichnis für verschiedene Benutzer angelegt wurde. 

An den vorgenannten Speicherorten können sich verschiedene Unterverzeichnisse befinden. War auf dem alten Server auch eine DaVinci Clientinstallation oder eine DaVinci Look, gibt es deutlich mehr Verzeichnisse.
Übertragen Sie diese Verzeichnisse bitte anstelle der gleichnamigen Verzeichnisse an die identischen Stellen auf dem neuen Server.

### Daten für den DaVinci InfoServer 

Speicherort:

* `C:\inetpub\wwwroot`

Wenn Ihr bisheriger Server auf für die Webpublikation per Webserver und DaVinci InfoServer verwendet wurde, denken Sie bitte daran zusätzlich noch diese Daten zu sichern. Wenn Sie keine eigenen Anpassungen an den Vorlagen vorgenommen haben, können Sie aber auch problemlos neue WebBox-Dateien auf dem neuen Server ablegen. Ein aktelles zip-Archiv mit den WebBox-Dateien finden Sie auf der Webseite [https://davinci-webbox.stueber.de/](https://davinci-webbox.stueber.de/).

## Anpassungen für die DaVinci Clients

Auf den Clientrechnern muss die Serververbindung auf den neuen Schulserver angepasst werden. Starten Sie dazu DaVinci, wenn das Programm versucht sich mit dem DaVinci Server zu verbinden, klicken Sie bitte auf `Abbrechen`. DaVinci öffnet sich, wechseln Sie bitte auf `Plan > Server verwalten`und öffnen im folgenden Fenster per Doppelklick auf Ihre Server-Verbindung die Eigenschaften. Passen Sie die Angaben in den Feldern `Netzwerkadresse`und ggfs. auch die `Port-Nummer`an.

Diese Angaben müssen bitte für alle DaVinci Clients wiederholt werden, alternativ kann man diese Angaben auch zentral verwalten, bitte lesen Sie dazu den Abschnitt [Die Pathsdatei](https://doc.davinci6.stueber.de/00.allgemein/pathdatei/).