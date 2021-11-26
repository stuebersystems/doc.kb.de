# Einrichtung/Installation der verschiedenen DAVINCI Komponenten

Für die sogenannten Serverrechner (im eigentlichen Sinne Rechner auf denen DAVINCI INFOSERVER, SERVER installiert und der Webserver eingerichtet werden) gilt:

Für die Einrichtung der Webbox gibt es letztlich drei Varianten, wovon die dritte die sicherste udn von uns empfohlene Variante ist:

1. Der DAVINCI Server, der DAVINCI INFOSERVER und Ihr Webserver sind auf einem gemeinsamen Server eingerichtet.
2. Der DAVINCI Server ist auf einem Server, der DAVINCI INFOSERVER und Ihr Webserver sind auf einem anderen Server, die Kommunikation zwischen beiden läuft über einen geöffneten Port.
3. Der DAVINCI Server ist auf einem Server, auf einem anderen Server sind ein weiterer DAVINCI Server, der DAVINCI INFOSERVER und Ihr Webserver. <br/><br/>In diesem Fall muss die Plandatei aus dem Arbeitsbereich und ggfs. auch die DAVINCI.users-Datei (enthält Ihre Benutzerverwaltung und die Plandateienstruktur des DAVINCI Servers) per FTP auf eine Stelle kopiert werden, von der diese Daten für den zweiten DAVINCI Server wieder abgeholt und zur Verfügung gestellt werden.<br/><br/>Dieser zweite DAVINCI Server dient einzig und allein der Publikation für die WEBBOX und die App. Diese dritte Variante kann mit Powershellskripten, die wir dazu zur Verfügung stellen, realisiert werden. Also die Skripte übernehmen den Übertrag der Informationen von Ihrem Schulserver auf den anderen Server. 
Eine Anleitung finden Sie dazu hier: https://doc.davinci6.stueber.de/09.infoserver/powershell/

## Was wird auf den Clients installiert

Auf den Arbeitsplätzen oder mobilen Endgeräten können Daten zur Information abgerufen werden. Zusätzlich können je nach Rolle des Nutzers auch Module zur Bearbeitung der Stundenplan- und/oder Vertretungsplandaten benötigt werden.

**DAVINCI WEBBOX**: Dient der Publikation der Daten, die der DAVINCI INFOSERVER bereitstellt. Für die Anzeige auf einem Rechner, Tablet oder Mobiltelefon genügt ein Webbrowser.

**DAVINCI MOBILE APP**: Dient der Publikation der Daten, die der DAVINCI INFOSERVER bereitstellt. Die App kann auf mobilen Endgeräten (Tablet oder Mobiltelefon) genutzt werden und wird für IOS oder Android angeboten.

**DAVINCI LOOK**: Kann auf windowsbasierten Rechnern installiert werden und kann zur reinen Information innerhalb der Schule oder mit direktem Zugriff auf das Schulnetzwerk genutzt werden. Die Daten werden direkt vom DAVINCI ENTERPRISE SERVER abgerufen.

**DAVINCI**: Kann auf windowsbasierten Rechnern installiert werden. Mit Hilfe dieses Moduls wird die Planung erstellt oder auch Vertretungen geregelt, die Ergebnisse können anschließend automatisch für DAVINCI LOOK DAVINCI WEBBOX oder die DAVINCI MOBILE APP präsentiert werden. Die Daten werden direkt vom DAVINCI ENTERPRISE SERVER synchronisiert.
