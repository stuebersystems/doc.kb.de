# Importlogik Magellan und DaVinci

## Schüler haben in Magellan keine zugewiesenen Fächer

Werden aus Magellan Schüler importiert, welche unter Schüler > zeugnis > Fächer noch keine Fächer hinterlegt haben, wird der Schüler nach Enbrea importiert und ist dort unter `Stammdaten > Schüler`mit der Klassenzugehörigkeit zu sehen und er ist der Klasse zugeordnet. Unter `Stammdaten > Klassen` ist der Schüler der Klasse zugeordnet aber keinen Kursen.

## Schülerwechsel in Magellan



## Kurszuordnung in Enbrea 

Unter `Stammdaten > Kurse` werden die Schüler je Kurs gezeigt. Dabei werden je nach eingesetzten Quellprogrammen (Schulverwaltung und Stundenplanung) Daten ausgewertet und die Schüler-Kurszugehörigkeit rückgeschlossen.

Damit das Rückschließen auf die Schüler je Kurs funktioniert, müssen die auszuwertenden Daten in den Quellprogrammen identisch gepflegt werden. Beispielsweise müssen die Fächer (Fachkürzel) im Stundenplanprogramm und in der Schulverwaltung gleich sein.

Werden aus der Schulverwaltung Daten zu Schülern und Klassen, aber keine Fächerangaben, importiert und liegen in der Stundenplanung (DaVinci oder UNTIS) keine Schülerdaten vor, dann werden im Enbrea Klassenbuch keine Kurszuweisungen vorgenommen. Diese müssen Sie nach dem Erstimport einmalig im Enbrea Klassenbuch pro Klasse machen. Bitte gehen Sie dazu in die Ansicht Unterricht > Klassen > Schülerzuweisung zu Kursen.

Nutzen Sie Magellan, muss die Kurszuweisung im Enbrea Klassenbuch nicht nachgepflegt werden. Hier kommt diese Zugehörigkeit direkt aus Magellan (Voraussetzung: gleiche Fachkürzel).

## Kurswechsel in DaVinci¶

Kommt es in DaVinci zu einem Kurswechsel bei einem Schüler, ist wird der Schüler nach der Änderung und dem Übertrag nach Enbrea in beiden Kursen geführt. Das Zu- und Abgangsdatum beim Kurswechsel muss in Enbrea selbst geändert werden unter Kurse.

## Neues Schuljahr¶

Arbeiten Sie nur mit dem Stundenplanprogram DaVinci und verwalten dort auch Ihre Schüler achten sie bitte unbedingt darauf zu Beginn eines neuen Schuljahres die Klassenzugehörigkeit der Schüler in DaVinci zu ändern Stammdaten > Schüler > Klasse.

## Schüler in mehreren Klassen¶

Schüler werden anhand der Information zu Vorname, Nachname, Geburtsdatum geprüft. Ist ein Schüler in DaVinci > Stammdaten > Schüler doppelt angelegt und unterscheidet sich nur in der DaVinci > Stammdaten > Schüler > Klasse wird der Schüler nur einmal in den Enbrea Stammdaten angelegt, aber beiden Klassen als Schüler zugeordnet.
Nebenlaufbahn eines Schülers¶

Hat eine Schüler in Magellan in Magellan eine Haupt- und Nebenlaufbahn Schüler > Auswahl > Laufbahn > H/N wird diese durch Klassenzugehörigkeit zu beiden Klassen in Enbrea mit den jeweiligen Zu- und Angangsdaten berücksichtigt.

## Fächer in Magellan und DaVinci

In der Regel haben Sie in DaVinci keine Schüler und Schülerinnen den Unterrichtsveranstaltungen zugewiesen. In Magellan haben die Schüler und Schülerinnen aber unter `Schüler > Zeugnis > Fächer` ihre zugewiesenen Fächer. Achten Sie darauf, dass Sie Magellan und DaVinci die gleichen Fachkürzel verwenden. In diesem werden werden die Schüler und Schülerinnen automatisch beim Datenimport nach Enbrea Klassenbuch den entsprechenden Kursen zugewiesen.

## Fach in DaVinci aber nicht in Magellan

In der Regel haben Sie in DaVinci keine Schüler und Schülerinnen den Unterrichtsveranstaltungen zugewiesen. Wurde dem Schüler oder der  Schülerin in Magellan unter `Schüler > Zeugnis > Fächer` ein Fach nicht zugewiesen, kann beim Datenimport nach Enbrea Klassenbuch den entsprechenden Kursen kein Schüler oder Schülerin zugewiesen werden. Sie können in diesem Fall im Enbrea Klassenbuch `Stammdaten > Kurse > Schülerzuweisung zu Kursen` machen. In diesem Fall werden alle Schülerinnen und Schüler der Klasse zugewiesen.

## Fach in DaVinci mit Gruppenteilung

Haben Sie ein Fach, welches in Teilung also in mehreren Gruppen unterrichtet wird, empfiehlt es sich, hier in DaVinci in Magellan die Fächer als Kurse also mit Kursnummern anzulegen. Durch die Zuordnung der Fächer mit Kursnummer in Magellan ensteht die Kurszuordnung der Schülerinnen und Schüler. Alternativ können Sie auch in DaVinci Schülerinnen oder Schüler der Veranstaltung zuweisen, dazu müssen aber in den `Stammdaten > Schüler` hinterlegt sein.

## Fächer in der gymnasialen Oberstufe

In der gymnasialen Oberstufe werden die Kursbildungen im DaVinci Kursplan gemacht. Das heißt hier werden die Zuordnungen der Schülerinnen und Schüler in DaVinci gemacht und automatisch beim Datenimport nach Enbrea Klassenbuch den entsprechenden Kursen zugewiesen.

## Emailadressen in Magellan und DaVinci

Haben Sie für Ihre Lehrkräfte in Magellan und DaVinci Emailadressen hinterlegt, die von einander abweichen, wird beim ersten Import nach der Importreihenfolge gegangen. Also gegebenefalls erst die Emailadresse aus DaVinci hinterlegt und dann geändert mit der in Magellan hinterlegten Emailadresse.

## Klassenwechsel in Magellan

## Ausschulen in Magellan

## Geblockte Veranstaltungen aus DaVinci

Blockungen können aus verschiedenen Gründen in DaVinci angelegt werden. In Enbrea werden geblockte Unterrichtsveranstaltungen als ein Elemnt für den Klassenbucheintrag betrachten und zwar in dem Fall wenn Lehrkraft und Zeit der geblockten Elemente gleich sind.

Exemplarisch könnte hiermit eine Wahlpflichtunterricht über verschiedene Klassen dargestellt werden

* 9a Bio Block WPU Lehrkraft A
* 9b Bio Block WPU Lehrkraft A
* 9c Bio Block WPU Lehrkraft A

Hierfür wird eine Klassenbucheintrag erstellt über alle 3 Klassen.

## Planwechsel in DaVinci

## Berfistung von Veranstaltungen in DaVinci

Die Befristung von Veranstaltungen wird in das Enbrea Klassenbuch übernommen. Auch Befristungen die Sie nachträglich machen werden übergeben. D.h. Veranstaltungen sind dann ggf. im Enbrea Klassenbuch ab einer bestimmten Kalenderweoche nicht mehr sichtbar.

## DaVinci 

Bitte prüfen Sie in DaVinci in den `Stammdaten > Lehrer` ob die Lehrkräfte Ihre Schule hier mit den entsprechenden korrekten Kürzeln, Vorname und Nachname und einer E-Mail-Adresse hinterlegt sind. Die hier hinterlegte E-Mail-Adresse wird später zur Kommunikation im Enbrea Klassenbuch benötigt.

Bitte prüfen Sie in DaVinci `Stammdaten > Klassen und Fächer` die Informationen Kürzel, Bezeichnung ggf. ID müssen mit den Daten Ihrer Schulverwaltung übereinstimmen. 

Wenn Sie Magellan und DaVinci gemeinsam einsetzen, so haben Sie den Vorteil, dass viele Daten nur einmal eingegeben werden müssen. Dadurch können Doppelerfassungen von Daten minimiert bzw. vermieden werden. Bitte beachten Sie dabei unsere Hinweis zum [Datenaustausch zwischen Magellan und DaVinci](https://doc.DaVinci6.stueber.de/11.datenaustausch/
Magellan/).

### Arbeit in der Gymnasialen Oberstufe Daten zu den Schülern werden in DaVinci erfasst

Um mit dem Enbrea Klassenbuch zu arbeiten, können Sie auch alle benötigten Daten nur im Planungsprogramm DaVinci nutzen. Die Klassen und Fächer werden in DaVinci erfasst, die Schüler und die Kurszuweisung. Diese wird durch den DaVinci Kursplan generiert.

Klassen erfassen Sie unter `Stammdaten > Klassen`

Fächer erfassen Sie unter `Stammdaten > Fächer`

Lehrkräfte erfassen Sie unter `Stammdaten > Lehrkräfte`

Schülerinnen und Schüler erfassen Sie unter `Stammdaten > Schüler` oder im Bereich `Kursplan > Schüler`

Die Erstellung der Kurs und die Kurszuordnung erfolgt im Bereich `Kursplan`.

### Kurswechsel in DaVinci

Kommt es in DaVinci zu einem Kurswechsel bei einem Schüler, wird der Schüler nach der Änderung und dem Übertrag nach Enbrea in beiden Kursen geführt. Das Zu- und Abgangsdatum beim Kurswechsel muss in Enbrea selbt geändert werden unter `Stammdaten > Kurse `

### Geänderter Stundenplan

Ändert sich der Stundenplan in Ihrer DaVinci Datei innerhalb des Zeitraumes von Enbrea geben Sie den Zeitraum der Gültigkeit des DaVinci Stundenplanes bitte in der DaVinci Plandatei unter `Plan > Eigenschaften > Zeitraum > Hauptzeitraum dieser Datei`an. Ab dem Startdatum werden die neuen Stundenplandaten nach Enbrea übertragen. Alle Termine vor dem Startdatum bleiben davon unberührt.

Arbeiten Sie mit einer lokalen DaVinci Datei müssen Sie diese nur wieder an der für dem Datenaustausch vorgesehenem Speicherpfad ablegen.

Arbeiten Sie mit einer Serverdatei muss die geänderte Datei auf den DaVinci Server geladen werden. Öffnen Sie das Modul `DaVinci Explorer` und rufen den Unterpunkt `Plandateien` auf. Laden Sie die vorbereitete Plandatei über die Schaltfläche `Hochladen` auf den bestehenden Platzhalter, welcher für die aktuelle Planung und gegebenenfalls auch für den DaVinci Infosever genutzt wird. 
Weitere Information dazu finden Sie [hier](https://doc.davinci6.stueber.de/06.enterprise/11.planwechsel/)

### Neues Schuljahr Schüler nur in DaVinci

Arbeiten Sie nur mit dem Stundenplanprogram DaVinci und verwalten dort auch Ihre Schüler achten sie bitte unbedingt darauf zu Beginn eines neuen Schuljahres die Klassenzugehörigkeit der Schüler in DaVinci zu ändern `Stammdaten > Schüler > Klasse`. 

### Schüler in mehreren Klassen

Schüler werden anhand der Information zu Vorname, Nachname, Geburtsdatum geprüft. Ist ein Schüler in `DaVinci > Stammdaten > Schüler` doppelt angelegt und unterscheidet sich nur in der `DaVinci > Stammdaten > Schüler > Klasse` wird der Schüler nur einmal in den Enbrea Stammdaten angelegt, aber beiden Klassen als Schüler zugeordnet.

## Magellan

Für den im Enbrea Klassenbuch zu bearbeitenden Zeitraum kommen die Informationen über die Zugehörigkeit der Schüler*innen zu bestimmten Fächern/Kursen einer Klasse aus Magellan. D.h. die Schüler müssen in diesem Zeitraum in Magellan den entsprechenden Klassen zugewiesen sein.

Wenn Sie Magellan und DaVinci gemeinsam einsetzen, so haben Sie den Vorteil, dass viele Daten nur einmal eingegeben werden müssen. Dadurch können Doppelerfassungen von Daten minimiert bzw. vermieden werden. Bitte beachten Sie dabei unsere Hinweis zum [Datenaustausch zwischen Magellan und DaVinci](https://doc.DaVinci6.stueber.de/11.datenaustausch/Magellan/).

### Nebenlaufbahn eines Schülers

Hat eine Schüler in Magellan in Magellan eine Haupt- und Nebenlaufbahn `Schüler > Auswahl > Laufbahn > H/N` wird diese durch Klassenzugehörigkeit zu beiden Klassen in Enbrea mit den jeweiligen Zu- und Angangsdaten berücksichtigt.

## Besonderheiten

### Unterscheidung Grund- und Leistungskurse

### Lernfeldunterricht

### Gruppenteilungen

#### Klasse teilt sich und die Gruppen haben unterscheidliche Fächer

#### Klasse teilt sich und die Gruppen haben das gleiche Fach aber bei anderen Lehrkräften

#### Klasse teilt sich und die Gruppen haben das gleiche Fach bei der gleichen Lehrkraft aber zu unterschiedliche Zeiten

### Unterricht in einem Fach wird von unterschiedlichen Lehrkräften unterrichtet

### Schüler werden in der Schule unterrichtet aber nicht in der Schulverwaltung geführt