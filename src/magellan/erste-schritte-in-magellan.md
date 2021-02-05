# Erste Schritte in MAGELLAN - leere Datenbank für den Echtbetrieb vorbereiten

``Stand Februar 2021``

Nach der Installation von MAGELLAN sind automatisch zwei Datenbanken hinterlegt.
Eine Beispieldatenbank, damit man sich anhand von Beispieldaten das Programm ansehen kann.
Und eine leere Datenbank mit der man in den Echtbetrieb wechseln kann.
Nachfolgend werden die Schritte beschrieben, die nötig sind um in den Echtbetrieb zu wechseln.

## Verbindung zur leeren Datenbank anlegen

Rufen Sie das Modul MAGELLAN ADMINISTRATOR auf. Um eine neue Verbindung anzulegen melden Sie sich als sysdba im Anmeldefenster an oder wählen im Anmeldefenster unter `Datenbank` `keine Anmeldung` aus. Mit dieser Anmeldung kann man die Verbindungsdaten einrichten oder korrigieren, falls versehentlich verkehrte Angaben vorgenommen wurden. Alle anderen Funktionen können ohne Anmeldung im MAGELLAN ADMINISTRATOR so nicht genutzt werden.

Der Unterschied zwischen der Beispielanbindung und dieser Anbindung ist letztlich vermutlich nur die Datenbank, insofern kann man die Beispielanbindung kopieren und anpassen. Wechseln Sie hierfür auf den Punkt `Datenbankverbindungen`, markieren die Beispielverbindung, klicken mit rechter Maustaste auf die Verbindung und wählen `Verbindung kopieren`.

![Verbindung kopieren](/images/magellan/04.png)

Passen Sie im nächsten Schritt den Namen des `Alias` an, diese Bezeichnung wird Ihnen später im MAGELLAN-Anmeldefenster gezeigt.

Anschließend wechseln Sie auf die Unterkarte `Datenbank` und passen den Datenbankpfad auf an. Bei einer Beispielverbindung wurde auf die Datenbank `Magellan8_Beispiel.fdb` verwiesen. Die leere Datenbank befindet sich im Datenbankverzeichnis neben dieser Datenbank und heißt `Magellan8.fdb`. Sie müssen also nur den Dateinamen von `Magellan8_Beispiel.fdb` auf `Magellan8.fdb` anpassen.

![Datenbanknamen anpassen](/images/magellan/05.png)

## Postleitzahlen importieren

Wählen Sie bitte unter `Datenaustausch > Postleitzahlen importieren` die Auswahl `Deutschland`. Sie erhalten ein vollständiges Postleitzahlverzeichnis für Deutschland, inklusive der Gemeindekennziffern u.a., das für statistische Erhebungen später wichtig ist.
Berliner Schulen importieren bitte das Postleitzahlverzeichnis `Berlin`, da hier zusätzlich die Berliner Stadtbezirke hinterlegt wurden. Für Schweizer Schulen steht ebenfalls ein Verzeichnis zur Verfügung.

## Schlüsselverzeichnisse importieren

Die Schlüsselverzeichnisse (zum Beispiel Fächer, Staatsangehörigkeiten, Noten u.a.) können unter dem Punkt `Datenaustausch > Schlüsselverzeichnisse importieren` in die leere Datenbank eingelesen werden.
Bitte wählen Sie: Ihre Region, wählen ob Sie Schlüssel für allgemeinbildende oder berufsbildende Schulen einlesen möchten, Ihre Schule und wählen bitte `alle Kataloge`.
Gibt es für Ihre Region kein Angebot, wählen Sie bitte als Wert `Deutschland`aus, damit werden die mindestens für MAGELLAN-Abläufe wichtigen Verzeichnisse gefüllt.

## Schulen importieren

In MAGELLAN können für Schüler Herkunftsschulen oder auch bei Abgängern die neue Schule vermerkt werden. Für einige Bundesländer gibt es auch eine vordefinierte Liste der Schulen, die nach MAGELLAN eingelesen werden kann.
Rufen Sie den Punkt `Datenaustausch > Daten über MAGELLAN-Importformat importieren` auf. Klicken Sie auf das Plus, wählen im der Verzeichnisstruktur Ihren Bundeslandunterordner aus (Standardpfad auf dem Server wäre `C:\Users\Public\Documents\Stueber Systems\Magellan 8\Importe`) und verweisen auf die Schulen.csv, die eingelesen werden soll. 
Definieren Sie die Datei in der Spalte `Importart` mit dem Wert `Schulen` und lesen die Datei ein.

![Schulen importieren](/images/magellan/06.png)

Steht für Ihre Region keine Schulendatei zur Verfügung, können Sie auch eine eigene Schulenliste auf diesem Weg einlesen. Wie diese Datei aufgebaut sein muss, beschreiben wir hier: [https://doc.magellan-toolbox.stueber.de/importe/MagImp/schnittstellenformat_schulenimportcsv/](https://doc.magellan-toolbox.stueber.de/importe/MagImp/schnittstellenformat_schulenimportcsv/).

## Zeiträume anlegen

Starten Sie MAGELLAN und wechseln zum Einrichten eines Zeitraumes bitte auf `Extras > Schlüsselverzeichnisse > Zeiträume`. Klicken Sie auf die Schaltfläche `Schuljahre anlegen` und stellen die Anzahl der zu erstellenden Schuljahre ein und klicken auf `OK`.

## Ihre Schuldaten eintragen

Wechseln Sie bitte in das Menü `Mandanten` und erzeugen über `STRG+N` oder über das Plus in der Menüleiste einen neuen Mandanten. Tragen Sie die mindestens ein Kürzel ein und klicken auf `OK`. Das Programm wechselt auf die Karte `Daten`, hier können Sie ausführlichere Schulinformationen erfassen.

## Daten erfassen

Sie können jetzt beginnen Ihre Schülerdaten einzutragen. Alternativ können Sie auch Daten aus entsprechend aufbereiteten csv-Dateien importieren., die notwendigen Schritte beschreiben wir im Dokument [https://doc.magellan-toolbox.stueber.de/](https://doc.magellan-toolbox.stueber.de/) Abschnitt [MAGELLAN-Importformat](https://doc.magellan-toolbox.stueber.de/importe/).
