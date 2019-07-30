# Eigene CSS-Vorlagen für Vertretungsplanapp in CONFIRE SHOWTIME verwenden

Öffnen Sie Ihre Projekt und wechseln zum Layout in das Sie die Vertretungsplanapp eingebunden haben. 
Auf der rechten Seite finden Sie unter `Design` die beiden Punkte `Eigene CSS` und `Eigenes Javaskript`.
Kopieren Sie den den Inhalt Ihrer angepassten CSS-Datei und fügen ihn unter `Eigene CSS` ein.

![Tragen Sie Ihre Änderungen unter Design in den Bereichen `Eigene CSS` und `Eigenes Javaskript` ein!](/images/infoserver/showt01.png)

Damit der Inhalt Ihrer CSS-Datei gelesen und geladen wird, kopieren Sie anschließend den nachfolgenden Text und fügen ihn unter `Eigenes Javaskript` ein.

```
var davinciElement=$(this);
function onLoad()
{ $(davinciElement.children("iframe")[0].contentDocument.body).append(davinciElement.children("style").clone()); }
function onElementStart(e)
{ davinciElement.children("iframe").on("load", onLoad); }
function onElementStop(e)
{ davinciElement.children("iframe").off("load", onLoad); }
function onElementDestroy(e)
{ davinciElement.children("iframe").off("load", onLoad); davinciElement.off("sht_element_start", onElementStart); davinciElement.off("sht_element_stop", onElementStop); }
davinciElement.on("sht_element_start", onElementStart);
davinciElement.on("sht_element_stop", onElementStop);
davinciElement.one("sht_element_destroy", onElementDestroy);
```

Starten Sie anschließend die Vorschau, Ihre Anpassungen sind nun auch in SHOWTIME sichtbar.

![Die grün gefärbte Leiste ergibt sich durch die Angaben unter `Eigene CSS` und `Eigenes Javaskript`!](/images/infoserver/showt02.png)