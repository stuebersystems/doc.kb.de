# Schuljahreswechsel

In diesem Artikel möchten wir Ihnen die verschiedenen Optionen erläutern, die Ihnen beim Schuljahreswechsel zur Verfügung stehen. Rufen Sie dazu über `Plan > Neu` den Planvorbereitungsassistenten auf.

Ihnen stehen drei Wege zur Verfügung.

![Wählen Sie einen Weg aus!](/sonstiges/schuljahreswechsel01.png)

**Neuen leeren Plan erstellen**

Dieser Weg ist für Neueinsteiger gedacht, die nicht auf einen Vorjahresplan aus DAVINCI zurückgreifen können.

**Neuen Plan erstellen und Daten übernehmen**

Diesen Weg wählen Schulen, die bereits auf eine Plandatei aus dem Vorjahr zurückgreifen und somit Daten übernehmen können.

**Neuen leeren Plan erstellen, aber aktuellen Planrahmen übernehmen**

## Neuen leeren Plan erstellen

Wählen Sie im Assistenten `Neuen Plan erstellen und Daten übernehmen` aus und geben Sie die Plandatei an, aus der Daten übernommen werden sollen. 

![Geben Sie an, aus welchem Plan die Daten übernommen werden sollen](/sonstiges/schuljahreswechsel02.png)

Klicken Sie auf `Weiter >`. Geben Sie nun an, ob es sich um einen Plan für das neue Schuljahre oder um einen Planwechsel innerhalb des Schuljahres handelt. Beim **Planwechsel innerhalb des Schuljahres** werden keine weiteren Änderungen an den Stammdaten vorgenommen.

![Geben Sie an, ob es sich um einen Plan für das neue Schuljahre oder um einen Planwechsel innerhalb des Schuljahres handelt](/sonstiges/schuljahreswechsel03.png)

> #### primary::Hinweis
>
> Die Klassenbezeichnungen bei Berufsbildenden Schulen bleibt davon unverändert. Generell gilt: Die Klassenstufe wird erhöht, die Klassen-IDs (falls vorhanden) werden gelöscht. Achten Sie bitte darauf, dass die zugewiesene Stundentafel, Klassenlehrer und Klassenraum unverändert bleiben. Dies müssen Sie in der neuen Plandatei entsprechend aktualisieren bzw. neu zuweisen.

Klicken Sie auf `Weiter `.

**Unterrichtsverteilung und Aufsichten löschen**

Wenn Sie diese Option wählen, werden nur die Stammdaten übernommen. Wahlweise können auch die Soll/Ist-Differenzen aus dem Vorjahr übernommen werden. Richten Sie dazu im Schlüsselverzeichnis „Lehrer-Soll-Schlüssel“ einen neuen Schlüssel mit dem Typ „D“ ein, den Sie beispielsweise „Übertrag aus letztem Schuljahr“ nennen. Richten Sie diesen Schlüssel noch im alten Plan, also vor der Datenübernahme, ein.

**Alles übernehmen**

Wenn Sie diese Option wählen, werden die Stammdaten, die Unterrichtsverteilung, die Aufsichten und die gesetzten Pläne übernommen.

![Wählen Sie, ob alles Übernommen werden soll oder die Unterrichtsverteilung und die Aufsichten gelöscht werden sollen](/sonstiges/schuljahreswechsel04.png)

Nachdem Sie nun eine dieser Optionen gewählt haben, klicken Sie auf `Weiter `. Es wird Ihnen eine Liste aufgezeigt, die Sie Schritt für Schritt durchgehen. 

![Liste der Schritte, die abzuarbeiten sind](/sonstiges/schuljahreswechsel05.png)

**1. Zeitraum eingeben...**

Über diese Schaltfläche gelangen Sie zu den Plan-Eigenschaften. Ändern Sie im Register „Zeitraum“ das Anfangs- und Enddatum für Ihren neuen Plan und bearbeiten Sie gegebenenfalls die Registerkarte „Statistik“ die Wochen. 

> #### primary::Hinweis
>
> In der Registerkarte "Zeitraum" können Sie als Startdatum das Datum des ersten Schultages und als Enddatum das Datum des letzten Schultages eingeben. Sie können es aber auch allgemein wie in unserem Beispiel halten. Durch den späteren Import des Ferienkalenders Ihres Bundeslandes wird Ihnen in der Plandatei der erste und letzte Schultag korrekt angezeigt.

![Plan-Eigenschaften, Register "Zeitraum"](/sonstiges/schuljahreswechsel06.png)

> #### primary::Hinweis
>
> In der Registerkarte "Statistik" nehmen Sie bitte im Bereich "Wochen" die Wochen heraus, in denen kein Unterricht stattfinden wird. Beachten Sie, dass hier nur ganze unterrichtsfreie Wochen ausgenommen werden dürfen. Der Import des Ferienkalenders hat auf die Markierung/Demarkierung der Kalenderwochen keinen Einfluss. Die Demarkierung der unterrichtfreien Wochen ist für die spätere Definition von Wochenbezügen (Perioden in DAVINCI) gedacht. Unterrichtsfreie Wochen werden somit standardmäßig mit jeder neuen Perioden, die Sie im Stammdatenfenster "Perdioden" definieren, voreingestellt.

![Plan-Eigenschaften, Register "Statistik"](/sonstiges/schuljahreswechsel07.png)

**2. Kalenderdaten imporieren...**

Über diese Schaltfläche können Sie den Ferienkalender für Ihr Bundesland importieren. Die aktuellen Kalenderdateien stellen wir Ihnen zur Verfügung. 

![Kalender importieren](/sonstiges/schuljahreswechsel08.png)


**3. Zeitrahmen einstellen...**

Für die Verplanung Ihrer Unterrichtstermine steht Ihnen ein Stundenraster zur Verfügung. Dieses Stundenraster wird durch die Unterrichtsstunden gebildet, deren Anzahl und Dauer Sie im Zeitrahmen festlegen. Gemeinsam mit den Unterrichts- und Pausenzeiten geben diese Angaben den Zeitrahmen vor, der Ihnen für die Terminplanung in den Wochenstundenplänen zur Verfügung steht. Bitte prüfen Sie die Eintragungen.

Standardmäßig gibt es einen Hauptzeitrahmen und einen Zeitrahmen für die Aufsichtsbereiche. In der Regel bleiben die Zeiten aus der Vorjahresplandatei unverändert, so dass Sie hier keine Änderungen vornehmen müssen. Neueinsteiger müssen hier Ihre Unterrichtszeiten und Pausenzeiten, die später beaufsichtigt werden, definieren.

![Zeitrahmen](/sonstiges/schuljahreswechsel09.png)


> #### warning::Wichtig!
>
> Bitte ändern Sie den Zeitrahmen nicht im Nachhinein an einem gesetzten Plan. Eine Änderung des Zeitrahmens hat keine Auswirkung auf verplante Termine, da diese mit Uhrzeit verplant werden.

**4. Stammdatenfenster...**

Passen Sie dann im Stammdatenfenster die Stammdaten an die neuen Gegebenheiten an (z.B. Klassen umbenennen, Klassen löschen oder neu anlegen usw.). Speichern Sie die neue Datei unter einem gewünschten Namen ab (standardmäßig wird von uns der Name "NeuerPlan.daVinci" vorgegeben).

## Gesetzte Termine löschen

Haben Sie im Planvorbereitungsassistenten die Daten aus der Vorjahresplandatei übernommen, können Sie die gesetzten Termine Ihres Planes ganz oder teilweise löschen.

Gehen Sie dazu wie folgt vor:

**Alle Termine einer/aller Klassen löschen**

Unter der Menügruppe `Automatik > Verplanungen zurücksetzen` oder unter `Start > Veranstaltungen > Löschen > Verplanungen zurücksetzen` können Sie gesetzte Termine aus dem Plan entfernen.

**Verschiedene Termine aus Plänen löschen**

Um einen bestimmten oder mehrere Termine wieder aus dem Plan zu entfernen, führen Sie bitte folgende Schritte aus: 
1. Markieren Sie das Terminfeld des zu entfernenden Termins. 
2. Betätigen Sie in der Menüleiste `Start > Stundenplan`  die Schaltfläche „Eintrag entfernen“. 
Der Termin wird nun aus dem Planungsfenster entfernt und befindet sich wieder in der Terminliste des „Unverplant“-Fensters.



