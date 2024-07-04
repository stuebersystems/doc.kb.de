# Postleitzahlen und Gemeinden aktualisieren

Einige Werte im Verzeichnis `Postleitzahlen` können sich zum Beispiel durch Gebietsrefomen verändern. Wenn das der Fall ist, erzeugen wir aus den Postleitzahlverzeichnissen der Post nach Magellan importierbare Dateien, legen diese per Update auf Ihrem Server ab und informieren darüber im Abschnitt "Was ist neu?" in der Magellan-Dokumentation. Diese Dateien müssen über das Modul Magellan Administrator in die Datenbank eingelesen werden. Anschließend müssen die eingelesenen Werte mit den in Ihrer Datenbank bereits verwendeten Werten abgeglichen werden. 

| Folgende Schritte sind notwendig         |
|------------------------------------------|
| 1. Postleitzahlverzeichnis importieren   |
| 2. Gemeinden synchronisieren             |
| 3. Vollständigkeit der Gemeindekennziffern für Schüler überprüfen |

## Postleitzahlverzeichnis importieren

Prüfen Sie bitte, ob in Ihrem Schulnetzwerk (Serverrechner und Arbeitsplatzrechner) die aktuellste Version eingesetzt wird.

### Importieren in Magellan 6

Öffnen Sie anschließend bitte im Magellan Administrator den Punkt `Datenimporte > Postleitzahlverzeichnis importieren`. 
Wählen Sie im Assistenten für `für folgendes Land` den Wert `Deutschland` aus und für `importiere folgenden Katalog` bitte `alle Kataloge`. Starten Sie den Assistenten über die Schaltfläche `Fertigstellen`.

### Importieren in Magellan 7 und 8

Öffnen Sie anschließend bitte im Magellan Administrator den Punkt `Datenaustausch > Postleitzahlen und Banken importieren`. 
Wählen Sie im Assistenten für `für folgendes Land` den Wert `Deutschland` aus und für `importiere folgenden Katalog` bitte `alle Kataloge`. Starten Sie den Assistenten über die Schaltfläche `Fertigstellen`.

## Gemeinden synchronisieren

Wenn das Einlesen der Postleitzahlen abgeschlossen ist, müssen die neuen Einträge im Verzeichnis mit den bestehenden Werten der Schüler, Lehrer, Schulen und Betriebe abgeglichen werden. Dabei wird die Postleitzahl und der Ort des jeweiligen Datensatzes (je Schüler, Lehrer usw.) mit den Inhalten des Postleitzahlverzeichnisses verglichen und falls eine Übereinstimmung vorliegt mit der Gemeindekennziffer ergänzt.

### Magellan 6

`Magellan Administrator > Datenbankpflege > Gemeinden synchronisieren`

Wenn die Postleitzahl und der Ort beim Datensatz mit einem Wert des Verzeichnisses übereinstimmt, dann wird die Gemeindekennziffer nachgetragen.
Der Eintrag erfolgt nur, wenn die Gemeinde eindeutig ist und noch keine Gemeindekennziffer hinterlegt wurde.
Die Aktion wird ausgeführt für:

* Schüler
* Betriebe
* Lehrer
* Schulen

### Magellan 7 und 8

`Magellan Administrator > Datenbankpflege > Datenbank überprüfen > Gemeindekennziffern synchronisieren`

Wenn die Postleitzahl und der Ort beim Datensatz mit einem Wert des Verzeichnisses übereinstimmt, dann wird die Gemeindekennziffer nachgetragen.
Der Eintrag erfolgt nur, wenn die Gemeinde eindeutig ist und noch keine Gemeindekennziffer hinterlegt wurde.
Die Aktion wird ausgeführt für:

* Schüler
* Betriebe
* Lehrer
* Sorgeberechtigte
* Schulen

## Vollständigkeit der Gemeindekennziffern für Schüler überprüfen

Sollte anhand der Postleitzahl und des Ortes zwischen den Schülern und dem Postleitzahlverzeichnis keine Übereinstimmung festgestellt werden, bekommt der Schüler keine Gemeindekennziffer zugewiesen.

In der Regel genügt die Korrektur des Schülerortes oder der Schüler-PLZ und ein erneuter Durchlauf des `Gemeinden synchronisierens`. Damit Sie einen Überblick haben, für welchen Schüler die Zuweisung nicht gelungen ist, finden Sie in `Magellan > Mandanden > Mandant markieren > Drucken` den Prüfbericht "Mandant (Ausgabe Schueler ohne Gemeindekennziffer).rpt". Rufen Sie pro Halbjahr diesen Bericht auf, es werden nur Schüler gezeigt, denen keine Gemeindekennziffer zugeordnet werden konnte.
