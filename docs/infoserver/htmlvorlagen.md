# DAVINCI INFOSERVER: HTML-Vorlagen mit "local" oder mit "main"?

> #### warning::Wichtig!
>
> Dieser Artikel bezieht sich auf die INFOSERVER-Ausgabe von HTML-Daten, im Gegensatz zur Nutzung der JSON-Daten für die DAVINCI-WEBBOX oder DAVINCI MOBILE erfolgt hierbei keine individuelle Benutzer-Autorisierung. **Wir empfehlen daher ausdrücklich den Einsatz der DAVINCI WEBBOX auf Ihren Webseiten.**



> #### primary::Hintergrund
>
> Der DAVINCI-Server übergibt dem Infoserver die Daten. Wie diese Daten aufbereitet sein sollen, entscheidet man mit der Auswahl der HTML-Vorlagen. Dabei gibt es Vorlagen mit "local" oder mit "main" im Dateinamen. Diese Bezeichnung unterscheidet von welcher Stelle weitere Informationen für die Anzeige abgeholt werden.
 
![DAVINCI > Publizieren > HTML-Pläne exportieren > HTML-Exportformate](../images/html_plaene_exportieren.png)


Folgende Dateien sind für die Ausgaben des Infoservers gedacht:


Name |Art der Anzeige|weitere Daten
---|---|---
davinci.index.main.html| Index| ergänzt mit Daten von unserem Server
davinci.index.local.html| Index| ergänzt mit Daten aus dem Verzeichnis sandbox im Rootverzeichnis Ihres Webservers
davinci.content.main.html|Stundenpläne| ergänzt mit Daten von unserem Server
davinci.content.local.html|Stundenpläne| ergänzt mit Daten aus dem Verzeichnis sandbox im Rootverzeichnis Ihres Webservers
davinci.showtime.subst.main.html|Vertretungsliste| ergänzt mit Daten von unserem Server
davinci.showtime.subst.local.html|Vertretungsliste|ergänzt mit Daten aus dem Verzeichnis sandbox im Rootverzeichnis Ihres Webservers



> #### primary::Wichtig
>
> Wenn Sie HTML-Vorlagen mit "local" in der Bezeichnung verwenden, zum Beispiel "DAVINCI.showtime.subst.local.html", werden die Dateien des Verzeichnisses "sandbox" im Rootverzeichnis Ihres Webservers erwartet.
Ein Verzeichnis "Sandbox" wird bei der Installation von DAVINCI mit erzeugt, Sie müssen es lediglich ins Rootverzeichnis Ihres Webservers kopieren. In der Regel sollte das Verzeichnis unter `C:\ProgramData\Stueber Systems\daVinci 6\HTML` zu finden sein. 


