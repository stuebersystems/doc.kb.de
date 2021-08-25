# Einrichtung/Installation der verschiedenen DAVINCI Komponenten

Für die sogenannten Serverrechner (im eigentlichen Sinne Rechner auf denen DAVINCI INFOSERVER, SERVER installiert und der Webserver eingerichtet werden) gilt:

Für die Einrichtung der Webbox gibt es letztlich drei Varianten möglich, wovon die dritte die sicherste ist und damit auch die empfohlene:
1.	Der DAVINCI Server, der DAVINCI INFOSERVER und Ihr Webserver sind auf einem Rechner(Schulserver).
D.h. auf diesem Rechner(Schulserver) sind DAVINCI INFOSERVER und DAVINCI SERVER installiert und ihr Webserver ist auf diesem eingerichtet.
2.	Der DAVINCI Server ist auf einem Rechner (Schulserver), der DAVINCI INFOSERVER und Ihr Webserver sind auf einem anderen Rechner, die Kommunikation zwischen beiden läuft über einen geöffneten Port.
D.h. auf dem Rechner(Schulserver) ist DAVINCI SERVER installiert. D.h. auf dem Rechner(Schulserver) ist DAVINCI SERVER installiert. Auf dem anderen Rechner ist DAVINCI INFOSERVER installiert und  ihr Webserver  eingerichtet.
3.	Der DAVINCI Server ist auf einem Rechner (Schulserver). Auf einem anderen Rechner sind ein weiterer DAVINCI Server, der DAVINCI INFOSERVER und Ihr Webserver.  In diesem Fall muss die Plandatei aus dem Arbeitsbereich und ggfs. auch die DAVINCI.users-Datei (enthält Ihre Benutzerverwaltung und die Plandateinenstruktur des DAVINCI Servers) per FTP auf eine Stelle kopiert werden, von der diese Daten für den zweiten DAVINCI Server wieder abgeholt und zur Verfügung gestellt werden. 
Dieser zweite DAVINCI Server dient einzig und allein der Publikation für die WEBBOX und die App. Diese dritte Variante kann mit Powershellskripten, die wir dazu zur Verfügung stellen, realisiert werden. Also die Skripte übernehmen den Übertrag der Informationen von Ihrem Schulserver auf den anderen Server. 
Eine Anleitung finden Sie dazu hier: https://doc.davinci6.stueber.de/09.infoserver/powershell/

Für die sogenannten Clientrechner (im eigentlichen Sinne Rechner auf denen DAVINCI oder DAVINCI LOOK installiert wird) gilt :

1.	Für Clients die sich nur in der Webbox anmelden benötigen Sie nur einen Browser um diese aufzurufen.
2.	Für Clients an denen Stunden- und Vertretungsplaner arbeiten, benötigen Sie nur eine DAVINCI Installation. Diese können dann aus dem Programm heraus mit dem Server und einer dort hinterlegten Datei verbunden werden.
3.	Für Clients an denen nur lesender Zugriff auf DAVINCI gewährt werden sollen, benötigen Sie nur eine DAVINCI LOOK Installation.
4.	Für Clients an denen Benutzer eingerichtet werden sollen und die Struktur der Planordner angelegt wird, sowie Dateien auf den DAVINCI Server geladen werden, benötigen Sie eine DAVINCI Installation. Mit der DAVINCI Installation wird der DAVINCI EXPLORER mit installiert, den Sie dafür benötigen.
