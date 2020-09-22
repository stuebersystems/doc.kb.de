# Welche Daten benötigen wir zum Einrichten des ENBREA-Testbetriebes

## Übermitteln der Daten

Bitte melden sich an der Weboberfläche (http://support.stueber.de) mit Benutzer (Ihre Mailadresse) und Passwort an, legen dort das Ticket mit dem Stichwort "ENBREA-Daten" im Titel an und laden die Daten direkt ins Ticket über die Schaltfläche "Durchsuchen". Auf diesem Weg können auch größere Dateien übermittelt werden, als es per Mail möglich wäre. 

## MAGELLAN Datenbank

Senden Sie uns bitte eine **Sicherungskopie** (*.fbk) Ihrer MAGELLAN Datenbank, vielen Dank!

Version|Vorgehen
--|--
MAGELLAN 6|Eine Sicherungskopie können Sie über den MAGELLAN -Administrator erstellen. Melden Sie sich bitte als sysdba (klappt aber auch ohne Anmeldung am Modul, Sie tragen die Anmeldung später beim Sichern ein) an und öffnen die Ansicht "Datensicherung". Tragen Sie die Anmeldungsdaten (sysdba und Passwort) ein und wählen einen Speicherort auf dem Serverrechner, der Name der Sicherung wird von MAGELLAN selbst vergeben.
MAGELLAN 7|Eine Sicherungskopie können Sie über den MAGELLAN -Administrator erstellen. https://doc.magellan7.stueber.de/schulverwaltung/admin/admin.datenbankverbindungen/#datensicherung

## DAVINCI Stundenplandatei

Einsatzart|Vorgehen
--|--
Serverbetrieb (ENTERPRISE)|Öffnen Sie bitte den `DAVINCI-EXPLORER > Plandateien`, wählen die entsprechende Datei aus und `Herunterladen`. Eine genaue Beschreibung dazu finden Sie [hier](https://doc.davinci6.stueber.de/06.enterprise/07.plandateien/#plan-herunterladen).
lokaler Betrieb|Senden Sie uns bitte die zuletzt bearbeitete DAVINCI Datei.
nur Schülerdaten aus DAVINCI|Sie können aus DAVINCI auch Schülerdaten exportieren, die nach ENBREA importiert werden können. Nähere Informationen dazu finden Sie [hier](https://doc.kb.stueber.de/enbrea/Sch%C3%BClerstammdaten%20importieren.html).

## edoo.sys RLP

Nutzen Sie die Schulverwaltung edoo.sys RLP schauen Sie bitte [hier](https://doc.kb.stueber.de/enbrea/export%20von%20Sch%C3%BClerdaten%20aus%20edoosys.html), wie Sie Schülerdaten inkl. Fächer mit unterrichtenden Lehrern exportieren können.

## Untis

Nutzen Sie zur Stundenplanung Untis, benötigen wir bitte folgende Daten:

* GPU001.TXT = Timetable data
* GPU002.TXT = Course data
* GPU003.TXT = Class data
* GPU004.TXT = Teacher data
* GPU005.TXT = Room data
* GPU006.TXT = Subject data
* GPU014.TXT = Substitutions data
* GPU018.TXT = Holiday data