# Einrichtung/Installation der verschiedenen DaVinci Komponenten

Für die sogenannten Serverrechner (im eigentlichen Sinne Rechner auf denen DaVinci InfoServer, Server installiert und der Webserver eingerichtet werden) gilt:

Für die Einrichtung der WebBox gibt es letztlich drei Varianten, wovon die dritte die sicherste udn von uns empfohlene Variante ist:

1. Der DaVinci Server, der DaVinci InfoServer und Ihr Webserver sind auf einem gemeinsamen Server eingerichtet.
2. Der DaVinci Server ist auf einem Server, der DaVinci InfoServer und Ihr Webserver sind auf einem anderen Server, die Kommunikation zwischen beiden läuft über einen geöffneten Port.
3. Der DaVinci Server ist auf einem Server, auf einem anderen Server sind ein weiterer DaVinci Server, der DaVinci InfoServer und Ihr Webserver. <br/><br/>In diesem Fall muss die Plandatei aus dem Arbeitsbereich und ggfs. auch die DaVinci.users-Datei (enthält Ihre Benutzerverwaltung und die Plandateienstruktur des DaVinci Servers) per FTP auf eine Stelle kopiert werden, von der diese Daten für den zweiten DaVinci Server wieder abgeholt und zur Verfügung gestellt werden.<br/><br/>Dieser zweite DaVinci Server dient einzig und allein der Publikation für die WebBox und die App. Diese dritte Variante kann mit Powershellskripten, die wir dazu zur Verfügung stellen, realisiert werden. Also die Skripte übernehmen den Übertrag der Informationen von Ihrem Schulserver auf den anderen Server. 
Eine Anleitung finden Sie dazu hier: https://doc.davinci6.stueber.de/09.infoserver/powershell/

## Was wird auf den Clients installiert

Auf den Arbeitsplätzen oder mobilen Endgeräten können Daten zur Information abgerufen werden. Zusätzlich können je nach Rolle des Nutzers auch Module zur Bearbeitung der Stundenplan- und/oder Vertretungsplandaten benötigt werden.

**DaVinci WebBox**: Dient der Publikation der Daten, die der DaVinci InfoServer bereitstellt. Für die Anzeige auf einem Rechner, Tablet oder Mobiltelefon genügt ein Webbrowser.

**DaVinci Mobile App**: Dient der Publikation der Daten, die der DaVinci InfoServer bereitstellt. Die App kann auf mobilen Endgeräten (Tablet oder Mobiltelefon) genutzt werden und wird für IOS oder Android angeboten.

**DaVinci Look**: Kann auf windowsbasierten Rechnern installiert werden und kann zur reinen Information innerhalb der Schule oder mit direktem Zugriff auf das Schulnetzwerk genutzt werden. Die Daten werden direkt vom DaVinci Enterprise Server abgerufen.

**DaVinci**: Kann auf windowsbasierten Rechnern installiert werden. Mit Hilfe dieses Moduls wird die Planung erstellt oder auch Vertretungen geregelt, die Ergebnisse können anschließend automatisch für DaVinci Look DaVinci WebBox oder die DaVinci Mobile App präsentiert werden. Die Daten werden direkt vom DaVinci Enterprise Server synchronisiert.
