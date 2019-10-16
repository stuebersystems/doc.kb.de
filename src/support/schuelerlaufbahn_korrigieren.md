# SchuelerLaufbahn korrigieren (MAGELLAN 7)

Um das Problem zu lösen führen Sie bitte die folgenden Schritte aus:

1. Laden Sie das Paket über den von unserem Supportteam in Ihrem Ticket übermittelten Link herunter.
2. Entpacken Sie das Zippaket über Rechtsklick|Extrahieren und öffnen anschließend das Verzeichnis "Schuelerlaufbahn korrigieren".

![Inhalt des Verzeichnisses](/images/support/schuelerlaufbahn_korrigieren/01.png)

3. In dem Verzeichnis befinden sich drei Dateien, starten Sie bitte per Doppelklick den MAGELLAN Skripteditor per Doppelklick auf die Datei "MagScriptEditor.exe".
4. Im Programmfenster gehen Sie bitte auf `Öffnen`!

![Öffnen](/images/support/schuelerlaufbahn_korrigieren/02.png)

5. Wählen Sie bitte wie nachfolgend die Datei aus und klicken anschließend auf `Öffnen`!

![Skript auswählen und öffnen](/images/support/schuelerlaufbahn_korrigieren/03.png)

6. Klicken Sie in das Fensterchen in dem das Wort `Quellcode` steht und schalten bitte in der Liste auf `Interface-Emulation` um.

![Auf Interface-Emulation umschalten](/images/support/schuelerlaufbahn_korrigieren/06.png)

7. Als nächstes brauchen Sie den Pfad zur Datenbank und ggfs. den Servernamen. Starten Sie dazu parallel  den MAGELLAN Administrator. Im Anmeldefenster melden Sie sich als sysdba an oder wählen falls Sie diese Zugangsdaten nicht parat haben, einfach `<keine Anmeldung>` aus.

![Administrator ggfs. ohne Anmeldung starten](/images/support/schuelerlaufbahn_korrigieren/04.png)

8.  Rufen Sie den Punkt `Datenbankverbindungen` auf und klicken bitte doppelt auf Ihre auf der rechten Seite angegebene Verbindung. Es öffnet sich das Fenster der Verbindungsdetails, Sie wählen die Unterkarte `Datenordner`.
![Administrator ggfs. ohne Anmeldung starten](/images/support/schuelerlaufbahn_korrigieren/05.png)
9. Sie benötigen den Eintrag aus dem Feld `Server` und den Eintrag aus dem Feld `Dateipfad aus dem Server`. Übernehmen Sie die Daten und tragen es plus dem sysdba-Passwort bitte im Skripteditor wieder ein.

![Eintragungen übernehmen](/images/support/schuelerlaufbahn_korrigieren/07.png)

Nachstehend eingetragene Beispieldaten: 

Vorlage|eingetragene Beispieldaten
--|--
const MagellanDatabase = 'Eintrag aus Dateipfad auf dem Server';|const MagellanDatabase = 'C:\Users\Public\Documents\Stueber Systems\Magellan 7\Datenbank\MAGELLAN7.fdb';
const MagellanUserName = 'sysdba';|const MagellanUserName = 'sysdba';
const MagellanPassword = 'Ihr Passwort';|const MagellanPassword = 'masterkey';
const Server = 'Eintrag aus dem Feld Server';|const Server = 'localhost';<br/>const Server = 'Verwaltungsserver';
const Protocol = 'TCP/IP';|

10. Sie lösen das Skript über das grüne Dreieck aus, das Skript überprüft die Schüler und meldet abschließend `Vorgang erfolgreich abgeschlossen`. Schließen Sie den Skripteditor, speichern ggfs. Ihre Angabe, schließen Sie den MAGELLAN Administrator und überprüfen in MAGELLAN das Ergebnis.

![Skript auslösen](/images/support/schuelerlaufbahn_korrigieren/08.png)

## Probleme

### Unable to complete network request...

````
Originaldateiname: Schullaufbahn gewechselt7.dws
Letzte Änderung: 05.09.2019
Copyright (c) 2019 STÜBER SYSTEMS GmbH
-------------------------------------------------------------------------------
Verbindung zu Datenbank aufbauen...
[FireDAC][Phys][FB]Unable to complete network request to host "IhrServername".
Failed to establish a connection.
[FireDAC][Comp][Clnt]-512. Verbindung ist nicht für [] festgelegt. Mögliche Ursache: Die Eigenschaftswerte von Connection und ConnectionName sind beide leer
Verbindung zur Datenbank abbauen...OK!
*** Vorgang mit Fehlern abgeschlossen ***
````

Sollte diese Meldung gezeigt werden, kann es ein Problem innerhalb Ihres Netzwerkes geben. Sie könnten statt des Servernamens die IP-Adresse des Serverrechners eintragen oder auch das Skript direkt auf dem Serverrechner ausführen und als Server dann `localhost` eintragen.