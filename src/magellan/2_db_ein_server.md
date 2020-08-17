# Zwei Datenbanken auf einen Server ablegen

Wenn Sie die Datenbanken zweier Schulen auf einem Server zusammen ablegen wollen, sollten Sie die folgenden Punkte beachten. 

## Version

Bitte stellen Sie sicher, dass beide Schulen die selbe Version von MAGELLAN und von Firebird einsetzen.

## Passworte der Nutzer

Die Benutzerkonten sind zum Teil in der MAGELLAN7.fdb der Schule angelegt, die verschlüsselten Passworte zu den Benutzern sind in einer zweiten Firebirddatenbank gespeichert die automatisch bei der Installation von Firebird angelegt wurde.  Wenn beide Datenbanken auf einem Rechner liegen, dann gibt es nur eine Firebirdinstallation, damit nur eine Passwortdatenbank (security2.fdb). Als erstes sollten Sie sich entscheiden welche der beiden Passwortdatenbanken Sie für den gemeinsamen Server übernehmen wollen. Es richtet sich sicher schlicht nach der Menge der angelegten Nutzer, also die Datenbank mit den meisten Nutzereinträge, deren security2.fdb wird mit auf den neuen Server übernommen. Wenn Sie identifiziert haben, welche Schule mehr Nutzer angelegt hat, dann kopieren Sie bitte die security2.fdb aus dem Firebirdverzeichnis und legen sie nach der Firebirdinstallation auf dem neuen Serverrechner anstelle der per Installation angelegten security2.fdb ab.
Ablagepfad bei Standardinstallation von Firebird: C:\Program Files (x86)\Firebird\Firebird_2_5

Wenn beide Schulverwaltungsdatenbanken (MAGELLAN7.fdb) übertragen wurde, melden Sie sich an der Datenbank an deren security2.fdb sie nicht übernommen haben und tragen die Passworte der Nutzer ein. Dazu klicken Sie bitte in der Benutzerverwaltung die Benutzer nacheinander doppelt an, tragen ein 8-stelliges Passwort (keine Umlaute, kein ß) ein und bestätigen. Durch das Ändern des Passwortes werden die Benutzer der Schulverwaltungsdatenbank damit in die jetzt gemeinsam genutzte Passwortdatenbank.

## sysdba und dbadmin

### sysdba

Der sysdba gilt als Administrator über alle Datenbanken auf dem Server, also in Ihrem Fall jetzt für beide Schulen, das Passwort sollten Sie ändern (MAGELLAN Administrator|Benutzerverwaltung|Administratoren) und den Schulen nicht mehr zur Verfügung stellen.

### dbadmin

Wenn die Schule selbst Nutzer anlegen darf, selbst Schlüssel für die eigene Datenbank importieren darf, also alle administrativen Aufgabe im MAGELLAN Administrator für die eigene Datenbank übernehmen darf, dann richten Sie bitte ein Passwort für den dbadmin der Schuldatenbank ein und stellen Sie diese Kennung den Schulen zur Verfügung.
Übrigens könnte somit auch jemand von der Schule die Passworte für die Benutzer anlegen.

### Datenordner

Bei den Datenordnern müssten Sie entscheiden, ob Sie Inhalte von den Schulen gemeinsam verwenden lassen oder es trennen wollen.
Unsere Empfehlung wäre folgende Konstellation, es sind aber sicher noch andere Varianten denkbar:

Muss je Schule existieren:

"C:\Users\Public\Documents\Stueber Systems\Magellan 7\Dokumente"

Sollten je Schule existieren:

"C:\Users\Public\Documents\Stueber Systems\Magellan 7\Berichte"

"C:\Users\Public\Documents\Stueber Systems\Magellan 7\Vorlagen"

Können gemeinsam genutzt werden:

"C:\Users\Public\Documents\Stueber Systems\Magellan 7\Skripte"

"C:\Users\Public\Documents\Stueber Systems\Magellan 7\Importe"

Unser Vorschlag hier wäre auf dem Server die Standardinstallation auszuführen und die Verzeichnis auch an der Stelle zu lassen. Für die schulindividuellen Verzeichnisse erstellen Sie bitte eine Kopie der Verzeichnisse ujnd legen diese doppelt ab. Erstellen Sie jeweils Freigaben für die beiden Schulen.
Bei Updates werden diese drei Verzeichnisse so nicht erreicht, was für die Verzeichnisse Dokumente und Vorlagen aber auch nicht nötig ist. Der Ordner Berichte sollte allerdings schon aktualisiert werden. Hier würden wir vorschlagen, dass Sie sich ein Tool zur Synchronisation des Verzeichnisses einrichten und nach dem Update neue oder geänderte Berichtsdateien aus dem Standardordner in die schulindividuellen Ordner zu übertragen.