# Umzug auf einen neuen Server

Für den Fall, dass Sie einen neuen Serverrechner anschaffen, finden Sie nachstehend eine Übersicht, der notwendigen Schritte.

> #### warning::Wichtig!
>
> Bitte aktualisieren Sie vorab auch bitte den alten DAVINCI auf die Version, mit der Sie Ihren neuen Server bespielen. Damit stellen Sie sicher, dass Daten, die übertragen werden gleich aktuell sind. 

## Installation des neuen Servers

Unsere Installationspakete finden Sie im  [Downloadbereich](https://davinci.stueber.de/download.php) 

Bitte führen Sie die gewünschten Installation aus, Anleitung dazu finden Sie hier: 

[DAVINCI Server](https://doc.davinci6.stueber.de/06.enterprise/01.installation/).
[DAVINCI](https://doc.davinci6.stueber.de/00.allgemein/installation/)
[DAVINCI LOOK](https://doc.davinci6.stueber.de/05.look/01.installation/)

Soll der DAVINCI INFOSERVER wieder eingerichtet werden, finden Sie die Anleitung von der Einrichtung des Webservers bis zur WEBBOX im Abschnitt [Live-DAten im Internet](https://doc.davinci6.stueber.de/internet-publication/).

## Lizenzierung

Wenn Sie nur den DAVINCI SERVER einrichten möchten, ist keine Lizenz auf dem Serverrechner nötig, die vorausgesetzte Lizenzierung wird über die DAVINCI Clients abgefragt. Lediglich wenn Sie den DAVINCI INFOSERVER verwenden, muss unter `Systemsteuerung (klassische Ansicht) > DAVINCI Server Control > Unterkarte Dienst > Schaltfläche Lizenz` eine entsprechende Lizenz eingetragen werden.

## Übernahme von Daten des alten Servers

> #### warning::Wichtig!
>
> Bevor Sie Daten auf den neuen Server übertragen, vergewissern Sie sich bitte, dass der "alte" DAVINCI SERVER-Dienst gestoppt wurde! Den Dienst können Sie unter `Systemsteuerung (klassische Ansicht) > DAVINCI Server Control > Unterkarte Dienst` stoppen.

### Verzeichnis Arbeitsbereich

Speicherort: `C:\Users\Public\Documents\Stueber Systems\daVinci 6\Arbeitsbereich`

Der Arbeitsbereich enthält die vom DAVINCI SERVER verwalteten Plandateien, mitunter Backup-Dateien und die DAVINCI.users-Datei, die die Benutzerverwaltung und die Plandateienstruktur des DAVINCI EXPLORERs.
 

Sollten Sie sich nicht sicher sein, an welcher Stelle sich Ihr Arbeitsbereichverzeichnis befindet, können Sie in dem Control (`Systemsteuerung (klassische Ansicht) > DAVINCI Server Control > Unterkarte Dienst`) auch auf der Unterkarte `Arbeitsbereich`nachsehen.

Dieses Verzeichnis legen Sie auf dem neuen Rechner nach der Installation unter dem Standardpfad ab, währenddessen muss der DAVINCI SERVER Dienst auf dem neuen Server gestoppt werden. Starten Sie ihn anschließend bitte wieder.


### weitere Verzeichnisses

Speicherorte: 

* `C:\Users\Public\Documents\Stueber Systems\daVinci 6\...`
* `C:\ProgramData\Stueber Systems\daVinci 6\...`
* `C:\Users\Ihr.Benutzer\AppData\Roaming\Stueber Systems\daVinci 6...` Bitte prüfen Sie, ob dieses Verzeichnis für verschiedene Benutzer angelegt wurde. 

An den vorgenannten Speicherorten können sich verschiedene Unterverzeichnisse befinden. War auf dem alten Server auch eine DAVINCI Clientinstallation oder eine DAVINCI LOOK, gibt es deutlich mehr Verzeichnisse.
Übertragen Sie diese Verzeichnisse bitte anstelle der gleichnamigen Verzeichnisse an die identischen Stellen auf dem neuen Server.


### Daten für den DAVINCI INFOSERVER 

Speicherort:

* `C:\inetpub\wwwroot`


Wenn Ihr bisheriger Server auf für die Webpublikation per Webserver und DAVINCI INFOSERVER verwendet wurde, denken Sie bitte daran zusätzlich noch diese Daten zu sichern. Wenn Sie keine eigenen Anpassungen an den Vorlagen vorgenommen haben, können Sie aber auch problemlos neue WEBBOX-Dateien auf dem neuen Server ablegen. Ein aktelles zip-Archiv mit den WEBBOX-Dateien finden Sie auf der Webseite [https://davinci-webbox.stueber.de/](https://davinci-webbox.stueber.de/).


## Anpassungen für die DAVINCI Clients

Auf den Clientrechnern muss die Serververbindung auf den neuen Schulserver angepasst werden. Starten Sie dazu DAVINCI, wenn das Programm versucht sich mit dem DAVINCI SERVER zu verbinden, klicken Sie bitte auf `Abbrechen`. DAVINCI öffnet sich, wechseln Sie bitte auf `Plan > Server verwalten`und öffnen im folgenden Fenster per Doppelklick auf Ihre Server-Verbindung die Eigenschaften. Passen Sie die Angaben in den Feldern `Netzwerkadresse`und ggfs. auch die `Port-Nummer`an.

Diese Angaben müssen bitte für alle DAVINCI Clients wiederholt werden, alternativ kann man diese Angaben auch zentral verwalten, bitte lesen Sie dazu den Abschnitt [Die Pathsdatei](https://doc.davinci6-kb.stueber.de/sonstiges/pathsdatei.html).