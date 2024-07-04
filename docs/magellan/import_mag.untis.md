# Magellan und Untis

Magellan unterstützt neben dem Datenabgleich zu unserem Stundenplanprogramm daVinci auch den Datenabgleich zum Stundenplanprogramm Untis. Dadurch können Sie mit Magellan und Untis arbeiten, ohne Daten doppelt eingeben zu müssen.

!!! info "Hinweis"

    Ein genauere Anleitung finden Sie in der Magellan-Dokumentation im Abschnitt [Datenabgleich Magellan und Untis](https://doc.magellan7.stueber.de/howto/stundenplaene.html#datenabgleich-magellan-untis).

Die Schnittstelle Magellan-Untis ist in Kooperation mit dem Hersteller von Untis entwickelt worden.
Der Datenabgleich kann entweder von Magellan nach Untis bzw. von Untis nach Magellan erfolgen. Im ersten Fall werden die Datenänderungen vom Stundenplaner in Untis mit Magellan abgeglichen. Im anderen Fall werden Veränderungen in Magellan auf die Daten in Untis übertragen.

Diese Funktion ist in Magellan ab dem Serviceupdate 5.1.7 und in Untis 2006 bzw. Untis 2007 ab der tagesaktuellen Version vom 29.09.06 verfügbar.

## Datenabgleich von Magellan nach Untis

Zum Austausch der Magellan-Daten mit Untis müssen Sie zunächst eine Schuldatentransferdatei in Magellan erzeugen, die dann in Untis eingelesen werden kann.

So exportieren Sie eine Schuldatentransferdatei für Untis aus Magellan:

1.	Wählen Sie in Magellan `Extras` und dann `Untis > Export`.
2.	Geben Sie die Magellan-Administrator-Kennung ein. Bestätigen Sie das Willkommen-Fenster.
3.	Wählen Sie im Fenster `Magellan-Export` den Mandanten und das Halbjahr, aus dem Sie die Daten übernehmen möchten. Zusätzlich müssen Sie die Schuldatentransferdatei (zum Beispiel SDTF.txt) angeben, in die Sie exportieren wollen.
4.	Wählen Sie die Daten aus, welche Sie nach Untis übertragen wollen.


Die aus Magellan exportierte Schuldatentransferdatei müssen Sie jetzt nur noch in Untis importieren:

1.	Starten Sie Untis mit Ihrer aktuellen Untis-Datei.
2.	Klicken Sie auf `Datei > Import/Export > Deutschland > Schuldatentransferformat`.
3.	Wählen Sie die Registerkarte `Importieren`. Geben Sie dort die aus Magellan exportierte Schuldatentransferdatei an, welche nach Untis importiert werden sollen. Klicken Sie dann auf `Importieren`.

## Datenabgleich von Untis nach Magellan

Um Daten aus Untis nach Magellan zu übertragen, müssen Sie in Untis zunächst eine Schuldatentransferdatei erzeugen, welche anschließend in Magellan importiert wird:

1.	Starten Sie Untis mit Ihrer aktuellen Untis-Datei.
2.	Klicken Sie auf `Datei > Import/Export > Deutschland > Schuldatentransferformat`.
3.	Wählen Sie die Registerkarte `Exportieren`. Geben Sie dort eine Exportdatei an, in welche die Untis-Daten exportiert werden sollen. Klicken Sie dann auf `Exportieren`.

Die aus Untis exportierte Schuldatentransferdatei muss nun nach Magellan importiert werden:

1.	Wählen Sie in Magellan `Extras` und dann `Untis > Import`.
2.	Geben Sie die Magellan-Administrator-Kennung ein. Bestätigen Sie das Willkommen-Fenster.
3.	Wählen Sie im Fenster Magellan-Import den Mandanten und das Halbjahr, in das Sie die Untis-Daten übernehmen möchten. Zusätzlich müssen Sie die Schuldatentransferdatei (SDTF-Datei) angeben, die Sie importieren wollen.
4.	Wählen Sie die Daten aus, welche Sie aus Untis übertragen wollen.
