# DaVinci InfoServer: Vertretungsliste soll flippen

Wir beschreiben es am Beispiel des Exportformates "Tagesvertretung nach Klassen mit Listflip" für den Parameter "daysubstclass".

Flippen kann eine Anzeige, wenn in der DaVinci.hfm, die der DaVinci-Server liest, eine entsprechende HTML-Vorlage gewählt wurde.

> #### primary::Hintergrund
>
> Der DaVinci-Server übergibt dem InfoServer die Daten. Wie diese Daten aufbereitet sein sollen, entscheidet man mit der Auswahl der HTML-Vorlagen. Alles was Sie im unten abgebildeten Programmbereich einstellen, wird in der DaVinci.hfm gespeichert.
 
![DaVinci > Publizieren > HTML-Pläne exportieren > HTML-Exportformate](/assets/images/html_plaene_exportieren.png)

Es gibt pro DaVinci-Installation eine solche Datei.

Man kann seine lokale Datei über den Punkt `HTML-Pläne exportieren` editieren und diese Datei dann auf den InfoServer-/DaVinci-Server-Rechner kopieren. Sollten der InfoServer und der DaVinci-Server auf  zwei verschiedenen Rechnern laufen, dann gehört die Datei auf den Rechner zum DaVinci-Server. An welcher Stelle der DaVinci Server die Datei liest, stellt man auf dem Server in der Systemsteuerung ein:

![Systemsteuerung > DaVinci-Server > InfoServer: Hier verweisen Sie auf die gewünschte DaVinci.hfm](/assets/images/hfm_fuer_server_einstellen.png) 

Oder:
Man installiert DaVinci auf dem Rechern mit dem DaVinci-Server und "biegt" den Pfad vom Servercontrol des DaVinci (hier steht an welcher Stelle DaVinci.hfm versucht wird zu lesen) auf die Stelle um, an der der DaVinci-Server die DaVinci.hfm liest. An welcher Stelle die DaVinci.hfm der DaVinci Installation liegt, sehen Sie in der DaVinci Oberfläche unter `Hilfe > Systeminformationen`.

![Systeminformationen für die DaVinci -Installation](/assets/images/speicherort_hfm-datei.png) 

Beim Einstellen selbst:
"daysubstclass" kann mit dem Exportformat "Tagesvertretungen nach Klassen" oder "Tagesvertretungen nach Klassen mit Listflip" hinterlegt sein. Sie wählen bitte die Variante mit Listflip. Das macht man, indem das Format in Spalte "Appname" mit IS hinterlegt wird.

> #### primary::Wichtig
>
> Es darf immer pro Typ nur ein Exportformat für den InfoServer markiert werden.

Markieren Sie nacheinander beide Zeilen, gehen jeweils auf Umbenennen und tippen IS in das Feld App-Name oder entfernen es.
 
![Per "Umbenennen" weisen Sie dem Exportformat den Wert "IS" zu.](/assets/images/appnamen_aendern.png)

Im Anschluss rufen Sie die Einstellungen des Listflip-Formates auf und stellen die HTML-Vorlage gemäß Abbildung ein. Nur die Vorlagen  mit dem Begriff "Showtime" im Namen können die Javadatei zum Flippen ausführen. 

Nur die mit "local" im Namen "interessieren" sich für Ihre Einstellungen, die Vorlagen mit "main" im Namen holen alle Infos von unserem Serverrechner ab. 

> #### primary::Wichtig
>
> Wenn Sie HTML-Vorlagen mit "local" in der Bezeichnung verwenden, zum Beispiel "DaVinci.showtime.subst.local.html", werden die Dateien des Verzeichnisses "sandbox" im Rootverzeichnis Ihres Webservers erwartet.

Schließen Sie im Anschluss den Dialog. Kopieren Sie nun die DaVinci.hfm auf den Pfad wie im DaVinci Servercontrol eingestellt. Falls die bearbeitete und die gelesene Datei identisch sind, ist das nicht nötig. 

Aber der DaVinci Server muss in jedem Fall neu gestartet werden, damit die Infos neu eingelesen werden können.

![Starten Sie abschließend den DaVinci Server bitte neu!](/assets/images/serverdienst_neustarten.png)
 

