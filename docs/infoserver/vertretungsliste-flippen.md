# DAVINCI INFOSERVER: Vertretungsliste soll flippen

Wir beschreiben es am Beispiel des Exportformates "Tagesvertretung nach Klassen mit Listflip" für den Parameter "daysubstclass".

Flippen kann eine Anzeige, wenn in der DAVINCI.hfm, die der DAVINCI-Server liest, eine entsprechende HTML-Vorlage gewählt wurde.

> #### primary::Hintergrund
>
> Der DAVINCI-Server übergibt dem Infoserver die Daten. Wie diese Daten aufbereitet sein sollen, entscheidet man mit der Auswahl der HTML-Vorlagen. Alles was Sie im unten abgebildeten Programmbereich einstellen, wird in der DAVINCI.hfm gespeichert.
 
![DAVINCI > Publizieren > HTML-Pläne exportieren > HTML-Exportformate](/assets/images/html_plaene_exportieren.png)

Es gibt pro DAVINCI-Installation eine solche Datei.

Man kann seine lokale Datei über den Punkt `HTML-Pläne exportieren` editieren und diese Datei dann auf den INFOSERVER-/DAVINCI-Server-Rechner kopieren. Sollten der Infoserver und der DAVINCI-Server auf  zwei verschiedenen Rechnern laufen, dann gehört die Datei auf den Rechner zum DAVINCI-Server. An welcher Stelle der DAVINCI Server die Datei liest, stellt man auf dem Server in der Systemsteuerung ein:

![Systemsteuerung > DAVINCI-Server > Infoserver: Hier verweisen Sie auf die gewünschte DAVINCI.hfm](/assets/images/hfm_fuer_server_einstellen.png) 

Oder:
Man installiert DAVINCI auf dem Rechern mit dem DAVINCI-Server und "biegt" den Pfad vom Servercontrol des DAVINCI (hier steht an welcher Stelle DAVINCI.hfm versucht wird zu lesen) auf die Stelle um, an der der DAVINCI-Server die DAVINCI.hfm liest. An welcher Stelle die DAVINCI.hfm der DAVINCI Installation liegt, sehen Sie in der DAVINCI Oberfläche unter `Hilfe > Systeminformationen`.

![Systeminformationen für die DAVINCI -Installation](/assets/images/speicherort_hfm-datei.png) 

Beim Einstellen selbst:
"daysubstclass" kann mit dem Exportformat "Tagesvertretungen nach Klassen" oder "Tagesvertretungen nach Klassen mit Listflip" hinterlegt sein. Sie wählen bitte die Variante mit Listflip. Das macht man, indem das Format in Spalte "Appname" mit IS hinterlegt wird.

> #### primary::Wichtig
>
> Es darf immer pro Typ nur ein Exportformat für den Infoserver markiert werden.

Markieren Sie nacheinander beide Zeilen, gehen jeweils auf Umbenennen und tippen IS in das Feld App-Name oder entfernen es.
 
![Per "Umbenennen" weisen Sie dem Exportformat den Wert "IS" zu.](/assets/images/appnamen_aendern.png)

Im Anschluss rufen Sie die Einstellungen des Listflip-Formates auf und stellen die HTML-Vorlage gemäß Abbildung ein. Nur die Vorlagen  mit dem Begriff "Showtime" im Namen können die Javadatei zum Flippen ausführen. 

Nur die mit "local" im Namen "interessieren" sich für Ihre Einstellungen, die Vorlagen mit "main" im Namen holen alle Infos von unserem Serverrechner ab. 

> #### primary::Wichtig
>
> Wenn Sie HTML-Vorlagen mit "local" in der Bezeichnung verwenden, zum Beispiel "DAVINCI.showtime.subst.local.html", werden die Dateien des Verzeichnisses "sandbox" im Rootverzeichnis Ihres Webservers erwartet.

Schließen Sie im Anschluss den Dialog. Kopieren Sie nun die DAVINCI.hfm auf den Pfad wie im DAVINCI Servercontrol eingestellt. Falls die bearbeitete und die gelesene Datei identisch sind, ist das nicht nötig. 

Aber der DAVINCI Server muss in jedem Fall neu gestartet werden, damit die Infos neu eingelesen werden können.

![Starten Sie abschließend den DAVINCI Server bitte neu!](/assets/images/serverdienst_neustarten.png)
 

