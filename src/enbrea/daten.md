# Welche Daten benötigen wir zum Einrichten des ENBREA-Testbetriebes

## Übermitteln der Daten

1. Bitte melden sich an der Weboberfläche (http://support.stueber.de) mit Benutzer (Ihre Mailadresse) und Passwort an.
2. Legen Sie dort bitte ein Ticket mit dem Stichwort "ENBREA-Daten" im Titel an.
3. Laden die Daten direkt ins Ticket über die Schaltfläche "Durchsuchen". Auf diesem Weg können auch größere Dateien übermittelt werden, als es per Mail möglich wäre. 

Nachstehend Hinweise für die benötigten Daten aus MAGELLAN, DAVINCI, edoo.sys, LUSD und Untis.

## MAGELLAN Datenbank

Senden Sie uns bitte eine **Sicherungskopie** (*.fbk) Ihrer MAGELLAN Datenbank, vielen Dank!

Version|Vorgehen
--|--
**6**|Eine Sicherungskopie können Sie über den MAGELLAN -Administrator erstellen. Melden Sie sich bitte als sysdba (klappt aber auch ohne Anmeldung am Modul, Sie tragen die Anmeldung später beim Sichern ein) an und öffnen die Ansicht "Datensicherung". Tragen Sie die Anmeldungsdaten (sysdba und Passwort) ein und wählen einen Speicherort auf dem Serverrechner, der Name der Sicherung wird von MAGELLAN selbst vergeben.
**7**|Eine Sicherungskopie können Sie über den MAGELLAN -Administrator erstellen. https://doc.magellan7.stueber.de/schulverwaltung/admin/admin.datenbankverbindungen/#datensicherung

## DAVINCI Stundenplandatei

Einsatzart|Vorgehen
--|--
Serverbetrieb (ENTERPRISE)|Öffnen Sie bitte den `DAVINCI-EXPLORER > Plandateien`, wählen die entsprechende Datei aus und `Herunterladen`. Eine genaue Beschreibung dazu finden Sie [hier](https://doc.davinci6.stueber.de/06.enterprise/07.plandateien/#plan-herunterladen).
lokaler Betrieb|Senden Sie uns bitte die zuletzt bearbeitete DAVINCI Datei.
nur Schülerdaten aus DAVINCI|Sie können aus DAVINCI auch Schülerdaten exportieren, die nach ENBREA importiert werden können. Nähere Informationen dazu finden Sie [hier](https://doc.kb.stueber.de/enbrea/Sch%C3%BClerstammdaten%20importieren.html).

## edoo.sys RLP

Wir haben Ihnen unter [folgendem Link](https://my.hidrive.com/share/8ey6i7s6ut) das Exportformat und die entsprechende Anleitung für den Export von Schülerdaten aus edoo.sys bereit gestellt. 
Die Anleitung und das Exportformat hat Herr Müller von der BBS Ahrweiler erstellt. Für den Export der Daten hat er das von Herrn Kiefer (edoo.sys Team) erstellte Exportformat um die Felder „Schüler_Stamm_ID" und "Alle Lehrkräfte mit Fach" ergänzt. Die so exportierten Daten (inkl. Fächer mit unterrichtenden Lehrern) benötigen wir für das elektronische Klassenbuch.

## Untis

Nutzen Sie zur Stundenplanung Untis, benötigen wir bitte folgende Daten:

* XML-Export (*.xml)
* GPU012.txt
* GPU013.txt [optional nötig, enthält Abwesenheitsgründe und Fehlzeiten der Lehrer]
* GPU014.txt

## LUSD

Nutzen Sie zur die LUSD, benötigen wir bitte folgende Daten:

* CSV-Exportdatei

Anleitung:

1. Rufen Sie den `Abfrageassistent` auf!

![](/images/enbrea/lusd01.png) 

1. Wählen Sie `Datenquelle > Kurse` aus! Klicken Sie auf `Hinzufügen` und vergeben Sie einen Namen für Ihre Abfrage.

![](/images/enbrea/lusd02.png) 
 
2. Fügen Sie Felder für Ihre Abfrage hinzu.
 
![](/images/enbrea/lusd03.png) 

3. Über die Lupe oben rechts im Fenster können Sie alle Schüler der Abfrage hinzufügen (`Auswählen > gewünschte Schulformen > Alle Übernehmen`)
6. Klicken Sie unten rechts im Fenster auf `Excel` um den Report aufzurufen.
 
![](/images/enbrea/lusd04.png) 