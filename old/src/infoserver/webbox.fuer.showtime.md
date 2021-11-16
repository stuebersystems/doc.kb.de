

# DAVINCI WEBBOX-Vertretungspläne auf E-BOARDs per CONFIRE SHOWTIME anzeigen

Die DAVINCI WEBBOX wird meist für die Anzeige von Stundenplan- und/oder Vertretungsplandaten (je nach Benutzerrecht) auf Ihrer Webseite verwendet. Sie können damit aber auch zum Beispiel Vertretungsplandaten auf Ihrem E-BOARD mit Hilfe von CONFIRE SHOWTIME anzeigen. Wir beschreiben Ihnen dafür einen Weg.

Was ist zu tun?

1. Benutzer anlegen
2. Benutzer dem Arbeitsbereich zuordnen
3. Richtlinien definieren
4. Mit CONFIRE SHOWTIME publizieren

## Benutzer anlegen

Wir empfehlen Ihnen einen Benutzer anzulegen, der nur für die Anzeige der Vertretungslisten in CONFIRE SHOWTIME verwendet wird. 
Melden Sie sich bitte mit Administrationsrechten am DAVINCI EXPLORER an und legen einen neuen Benutzer (ohne Administrationsrechte) an.
 
![Legen Sie einen neuen Benutzer an](../images/infoserver/infoserver.07.png)

## Benutzer dem Arbeitsbereich zuordnen und Richtlinien definieren

Ordnen Sie diesen Benutzer bitte auf der Karte `Plandateien` dem Arbeitsbereich zu und vergeben bitte die Richtlinien für den INFOSERVER entsprechend Ihrer Vorstellungen. Für die Anzeige des Vertretungsplans empfehlen wir folgende Angaben:

![Ordnen Sie den Benutzer dem Arbeitsbereich zu und vergeben die Richtlinien](../images/infoserver/infoserver.05.png)

> #### primary::Hinweis
>
> Die Vergabe der Richtlinien auf Höhe des Arbeitsbereiches ist kein Problem, da per Webbox generell nur auf die Plandatei zugegriffen werden kann, die im Control des DAVINCI INFOSERVERs (in der Systemsteuerung) hinterlegt wurde.

## Mit CONFIRE SHOWTIME publizieren

CONFIRE SHOWTIME dient zum zeitgesteuerten (auch benutzerverwalteten) Definieren (mit dem Designer) und Anzeigen (mit dem Player) verschiedenster Inhalte (Bildersammlungen, Texten, Videos, Webseiten, Apps usw. ). Für die Anzeige der Vertretungs- oder Stundenplandaten aus DAVINCI gibt es eine fertige App im Designer. 
Sie müssen nichts weiter tun, als Ihrem Projekt ein weiteres Layout hinzuzufügen. In dem Layout ergänzen Sie zwei Vertretungslistenapps. Sie finden dies Möglichkeit in der Leiste am oberen Bildrand unter `Layout > Apps > DAVINCI > Vertretungsliste`.
 
> #### warning::Wichtig!
>
> Diese CONFIRE SHOWTIME App ist perfekt auf die WEBBOX-Inhalte abgestimmt und besitzt bereits fertige Einstellmöglichkeiten für: Inhalte, Refreshintervalle, Flipintervalle und verschiedene Layouteinstellungen.


![Fügen Sie die Vertretungslistenapp ein und positionieren sie in Ihrem Layout](../images/infoserver/infoserver.04.png)

Feld|Eintrag
---|---
URL|Auf der rechten Seite finden Sie die Einstellungen für die eingefügte App. Tragen Sie dort die URL ein. In unserer Abbildung steht dort "localhost", bei Ihnen könnten innerhalb Ihres Netzwerkes, die interne IP-Adresse des Rechners auf dem der INFOSERVER läuft stehen. Außerhalb könnte es die öffentliche IP-Adresse  des Rechners sein oder eine Webseite mit Namensbindung.
Benutzer<br/>Kennwort|Tragen Sie bitte hier die Zugangsdaten Ihres im DAVINCI EXPLORER erfassten Benutzers an.
Weitere Parameter|Sie haben die Möglichkeit die Parameter, die wir unter [https://davinci-webbox.stueber.de/](https://davinci-webbox.stueber.de/) beschreiben, auch hier zu verwenden.<br/><br/> Im Beispiel verwenden wir den Parameter `substitutionShowExtra` mit dem Wert `none`, um pro Anzeige tatsächlich nur die Daten eines Tages auszugeben.

![Vertretungsplanapp mit den Einstellungen für "Heute"](../images/infoserver/infoserver.08.png)


![Vertretungsplanapp mit den Einstellungen für "Morgen"](../images/infoserver/infoserver.09.png)



> #### danger::Achtung!
>  
> Bitte den Parameter useSSL=true verwenden, um Daten von einem Https-Server anzeigen zu können.