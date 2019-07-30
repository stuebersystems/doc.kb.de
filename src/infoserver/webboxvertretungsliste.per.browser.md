## WEBBOX-Vertretungsliste per Browser für E-BOARDs publizieren

Der DAVINCI INFOSERVER fragt Daten vom DAVINCI ENTERPRISE Server ab und übergibt sie an die WEBBOX. Die WEBBOX besteht aus fix und fertig konfigurierten HTML-Seiten, die Stundenplan- und Vertretungsplaninhalte ansprechend aufbereiten. 
Die WEBBOX kann in einen Bereich Ihrer Webseite integriert werden, es könnten Inhalte ohne Anmeldung sichtbar sein (je nach Einstellung aber auch nicht), es gibt Inhalte die erst nach der Anmeldung des Nutzers (Klassen, Lehrer, Schüler, Eltern, Ausbilder...) sichtbar sind. 

Zusätzlich können Sie aber auch die Ausgaben der WEBBOX für die Anzeige des Vertretungsplans verwenden:

* eingebunden mit weiteren Inhalten in ein CONFIRE SHOWTIME-Projekt, eine Anleitung finden Sie [hier](https://doc.davinci6-kb.stueber.de/infoserver/webbox.fuer.showtime.html). 
* Anzeige in einem Browser auf einem E-BOARD

Die Anzeige im Browser kann man nutzen, um auf E-BOARDs im Browserfenster die aktuellen Vertretungsdaten anzeigen zu lassen. Damit ist allerdings nur die Anzeige einer Liste möglich, möchten Sie gern mehrere Liste mit unterschiedlichen Inhalten zeigen (zum Beispiel links die Vertretungsdaten von heute, rechts die von morgen plus zusätzliche Inhalte), verwenden Sie bitte unter Programm zur zeit- und auch benutzergesteuerten Anzeige von digitalen Inhalten CONFIRE SHOWTIME.



Für die Anzeige im Browser muss folgendes vorbereitet werden:
* ein Benutzer mit den entsprechenden Rechten
* einen Link mit passenden Parametern

## Benutzer anlegen

Wir empfehlen Ihnen einen Benutzer anzulegen, der nur für die Anzeige der Vertretungslisten im Browser verwendet wird. 
Melden Sie sich bitte mit Administrationsrechten am DAVINCI EXPLORER an und legen einen neuen Benutzer (ohne Administrationsrechte) an.
 
![Legen Sie einen neuen Benutzer an](/images/infoserver/infoserver.10.png)

## Benutzer dem Arbeitsbereich zuordnen und Richtlinien definieren

Ordnen Sie diesen Benutzer bitte auf der Karte `Plandateien` dem Arbeitsbereich zu und vergeben bitte die Richtlinien für den INFOSERVER entsprechend Ihrer Vorstellungen. Für die Anzeige des Vertretungsplans empfehlen wir folgende Angaben:

![Ordnen Sie den Benutzer dem Arbeitsbereich zu und vergeben die Richtlinien](/images/infoserver/infoserver.11.png)

> #### primary::Hinweis
>
> Die Vergabe der Richtlinien auf Höhe des Arbeitsbereiches ist kein Problem, da per Webbox generell nur auf die Plandatei zugegriffen werden kann, die im Control des DAVINCI INFOSERVERs (in der Systemsteuerung) hinterlegt wurde.

## Den Link zusammenstellen

Ein fertiger Link könnte zum Beispiel (sämtliche Parameter finden Sie unter [https://davinci-webbox.stueber.de/](https://davinci-webbox.stueber.de/)) so aussehen:


```
.../davinci-substitutions.html?username=blackboard.user&password=blackboard.user.password&dateOffset=1&substitutionShowExtra=none&substKey=teacher&substCols=date|weekDay|pos|time|steacher|teacher|subject|room|class|caption&refreshInterval=300000&flipInterval=5000

```

### Was ist in diesem Link enthalten?

Teil der URL|Bedeutung
---|---
...|Steht als Platzhalter für die Adresse des Rechners, auf dem der DAVINCI INFOSERVER läuft
username=blackboard.user<br/>password=blackboard.user.password|sind die Anmeldedaten, mit denen die Vertretungsdaten abgeholt werden
davinci-substitutions.html|ruft die von uns für die reine Anzeige von Vertretungsdaten zur Verfügung gestellte HTML-Seite aus dem Rootverzeichnis Ihres Servers auf. Alle folgenden Parameter sind optional, die HTML-Seite zeigt ohne weitere Parameter den von uns vorgegebenen Standard.
dateOffset=1<br/> oder<br/>dateOffset=0|der Parameter dateOffset wird verwendet, um den Starttag zu definieren. 0 bedeutet ab heute, 1 bedeutet ab morgen. Wenn heute Freitag ist und Ihr Plan nur Inhalte von Montag bis Freitag beinhaltet, dann steht die 1 allerdings für ab dem nächstmöglichen Tag, in diesem Beispiel wäre das dann ab Montag.
substitutionShowExtra=none|Dieser Parameter verhindert, dass außer den Inhalten des einzelnen Tages noch weitere im Fenster gezeigt werden. <br/>Beispiel:`dateOffset=0&substitutionShowExtra=none` gibt nur die Daten von heute aus.
substKey=teacher|Sortiert die Daten innerhalb des Tages nach den Lehrern [möglich wäre auch class, der Standard ist time]
substCols=...|Hiermit können Sie Spalten durchs Weglassen ausblenden, die Reihenfolge in der URL entspricht der Reihenfolge in der Anzeige.
refreshInterval=300000|Sie definieren hier in Millisekunden in welchen Intervallen der INFOSERVER den DAVINCI Server nach Änderungen fragt
flipInterval=5000|Passen nicht alle Änderungen in eine Liste, blättert die Liste seitenweise weiter. Stellen Sie über diesen Parameter ein, in welcher Geschwindigkeit die Seiten geblättert werden sollen. Wert in Millisekunden
