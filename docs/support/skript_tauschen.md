# Skript austauschen

[1]:/assets/images/admin.ohne.anmeldung.png "ohne Anmeldung starten"
[2]:/assets/images/skriptepfad.png "Skriptepfad kopieren"

!!! warning Wichtig

    Eine Skriptdatei kann in der Regel auch ohne Update getauscht werden, dafür muss mindestens die eingesetzte Versionsnummer stimmen. Beispielsweise kann ein Magellan 9-Skript nicht mit Magellan 6 eingesetzt werden oder umgekehrt.

Skripte liegen in der Regel auf dem Schulserver, nicht auf dem lokalen Clientrechner des Nutzers. Durch Freigaben kann dieses Verzeichnis aber auch von den Arbeitsplätzen der Nutzer aus erreicht werden, Sie müssen also nicht direkten Zugriff auf den Serverrechner haben.

## Allgemeines Skript oder regionales Skript?

Es gibt allgemeine Skripte, die in das Verzeichnis "Skripte" gehören oder regionale Skripte, die in das Verzeichnis "Skripte/"Meine Region" gehören.

Skripttyp|Ablage
--|--
Allgemeines Skript | Wenn es sich um ein allgemeines Skript handelt (bspsw. `Schüler einschulen.dws`), dann ersetzen Sie damit bitte die gleichnamige Datei direkt im Skripteverzeichnis. 
Berechnungsskript|Wenn es sich beispielsweise um ein Berechnungsskript (beginnend mit einem Regionalkürzel, bspsw. `SAC-BG-APO-2021.dws`) handelt, dann muss die Datei in den jeweiligen Regionalordner abgelegt werden, in diesem Beispiel in das Verzeichnis `Sachsen`.

## Austausch

Das von Ihrer Magellan-Instanz verwendete Skripte-Verzeichnis finden Sie auf folgende Weise:

1. Öffnen Sie das Modul `Magellan Administrator` auf Ihrem Rechner ohne Anmeldung!
![ohne Anmeldung starten][1]
2. Wechseln Sie auf `Datenbankverbindungen` und doppelklicken Sie auf die Verbindung, die Sie in der Regel starten um sich an Magellan anzumelden, in der Regel heißt diese Verbindung schlicht "Magellan".
3. Im sich öffnenden Unterfenster wählen Sie den Punkt `Datenordner`.
4. Markieren Sie den Pfad in der Zeile `Skripte` und kopieren Sie ihn in die Zwischenablage (`STRG+C`).
![Skriptepfad kopieren][2]
5. Schließen Sie ohne Veränderung das Verbindungsfenster und den `Magellan Administrator`!
6. Öffnen Sie ein beliebiges Ordnerfenster (`Windows-Taste+E`) und fügen den kopierten Pfad in die Adressleiste des Fensters (`STRG+V`).
7. Drücken Sie die `Entertaste`, es öffnet sich das Skripteverzeichnis auf dem Schulserver.
8. Entpacken Sie ggfs. die Zip-Datei und kopieren jetzt die enthaltene Skriptdatei oder die Dateien in die Zwischenablage (`STRG+C`) und fügen die Datei entweder direkt ins Skriptverzeichnis (Allgemeines Skript) oder in ein regionales Unterverzeichnis (Berechnungsskript) ein. Die genaue Ablage ist wichtig, bitte lesen Sie den nachstehenden Abschnitt.

