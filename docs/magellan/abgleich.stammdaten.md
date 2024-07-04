# Magellan und DaVinci: Fächer abgleichen

> #### danger::Achtung!
>
> Wenn zwischen beiden Programmen abgeglichen werden soll, müssen bestimmte Daten im jeweils anderen Programm identifiziert werden können. Dazu müssen die Kürzel, teilweise auch die IDs (es handelt sich um die aus Magellan nach DaVinci übergebene ID) identisch sein. Wir beschreiben den Abgleich nachstehend am Beispiel Fächer. Je nachdem was übergeben werden soll, müssen auch Klassenkürzel, Fachstatuskürzel, Unterrichtsartenkürzel, Lehrerkürzel, Schülervor- und Schülernachnamen gleich gepflegt sein.

**Problem:**

Sie möchten zwischen Magellan und DaVinci Daten abgleichen, zum Beispiel die Fachwahl Ihrer Oberstufenschüler, erhalten aber ein ähnliche Meldung wie nachstehend? 

```
Verbindung zu Magellan aufbauen...OK!
Textzeile importieren (3428)...
Einzulesendes Fach "PH" in nachfolgender Zeile existiert nicht in Magellan.
Einzulesendes Fach "SP" in nachfolgender Zeile existiert nicht in Magellan.

```
**Lösung:**
Der Abgleich basiert auf den Kürzeln und ggfs. den IDs der Fächer in beiden Programmen, sind diese gleich, können Daten abgeglichen werden. Diese Daten müssen also vereinheitlicht werden. Das kann per Hand oder per Abgleich geschehen. 

> #### warning::Wichtig!
>
> Bitte passen Sie jeweils nur die vorhandenen Zeilen an, löschen Sie bitte nichts! Mit den Fächern sind vielleicht Unterricht oder die Fachwahl eines Schülers usw. verbunden. 

## manuelle Anpassung

Nur als Beispiel: Es wird bemängelt, das die Fächer "PH" und "SP" nicht existiert. Bitte schauen Sie in DaVinci unter `Stammdaten > Fächer` nach:
* Gibt es PH (bitte achten Sie auch auf Groß- und Kleinschreibung)?
* Hat das Fach eine ID, wenn ja welche (diese wird wenn dann aus Magellan hierher übergeben)?

Schauen Sie analog dazu in Magellan unter `Verzeichnisse > Fächer` nach, gibt es PH und wie ist die ID?
Vermutlich gibt es hier Ungleichheiten, die genau zu diesen Meldungen führen.

Gehen Sie die Fächer in den Programmen nach Fehlermeldungen einzeln durch und korrigieren die Ungleichheiten.

> #### warning::Wichtig!
>
>  Die Fächer in Magellan sind in der Regel die, die durch den Import der Schlüsselverzeichnisse den korrekten Statistikschlüssel haben. Wir empfehlen daher in diesen Fall nicht den Übertrag der Fächer von DaVinci nach Magellan - geändert werden bitte lediglich die Stammdaten in DaVinci.

## Anpassen per Abgleich

### Löschen der Stammdaten-IDs

Leeren Sie als erstes in DaVinci das Feld ID beim Fach unter `Stammdaten > Fächer`. Diese Daten werden beim anschließenden Einlesen der Fächer aus Magellan aufgefüllt, bleibt eine ID frei, wissen Sie direkt, dass es das Fach nicht in Magellan gibt.

![Stammdaten > Fächer > Extras > Weitere Aktionen > Stammdaten IDs löschen](/assets/images/abgleich.00.png)

### Übertrag/Abgleich der Fächer aus Magellan

Lesen Sie die Fächer aus Magellan ein. Sie führen hierfür folgende Schritte aus:

Rufen Sie `Plan > Importieren und Exportieren > Importieren > von Magellan importieren` auf.


![Melden Sie sich an der Magellan-Verbindung an!](/assets/images/abgleich.01.png)




Melden Sie sich an der Magellan-Verbindung an!


![Haken Sie bitte nur den Punkt "Übernehme Fächer" an!](/assets/images/abgleich.02.png)

Bitte haken Sie nur den Punkt "Übernehme Fächer" an!

![Stammdaten > Fächer > Extras > Weitere Aktionen > Stammdaten IDs löschen](/assets/images/abgleich.03.png)

Es werden alle Fächer aus dem Magellan-Verzeichnis Fächer übernommen. 

> #### primary::Hinweis
>
> Eine Ausnahme stellen die Fachzeilen dar, die im Magellan-Verzeichnis Fächer mit "kein DaVinci-Abgleich" gekennzeichnet sind.

Was|Folge
---|---
Ein Fach wird anhand des identischen Kürzels erkannt| die ID  und weitere Daten (Schlüssel, Fachkategorie, Aufgabenbereich usw) aus Magellan werden in DaVinci unter `Stammdaten > Fächer` am bestehenden Fach ergänzt
Fachkürzel und ID sind in DaVinci vorhanden|weitere Daten (Schlüssel, Fachkategorie, Aufgabenbereich usw) aus Magellan werden in DaVinci unter `Stammdaten > Fächer` am bestehenden Fach ergänzt
Kürzel ist gleich, ID ist verkehrt| bestehendes Fach wird nicht geändert, neues Fach nicht angelegt, da das Kürzel eindeutig sein muss


### Ergebnis prüfen

Prüfen Sie anschließend bitte die Fächerliste in DaVinci unter `Stammdaten > Fächer`. Zeilen, die keinen Eintrag in der Spalte ID haben, haben bislang keine Entsprechung in Magellan. 

Fach fehlt in Magellan|Das kann ein Versehen sein, legen Sie das Fach in Magellan bitte an, verwenden das identische Kürzel und prüfen Sie, ob gegebenenfalls ein Statistikschlüssel im Feld Schlüssel erfasst werden muss.
Fach existiert in Magellan mit einem anderen Kürzel| Ändern Sie das Kürzel auf den Wert, der in Magellan verwendet wird, tragen Sie die ID nach oder gleichen erneut ab

