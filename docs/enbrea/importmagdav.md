# Importlogik Magellan und DaVinci

## Kurszuordnung in Enbrea 

Unter `Stammdaten > Kurse` werden die Schüler je Kurs gezeigt. Dabei werden je nach eingesetzten Quellprogrammen (Schulverwaltung und Stundenplanung) Daten ausgewertet und die Schüler-Kurszugehörigkeit rückgeschlossen.

Damit das Rückschließen auf die Schüler je Kurs funktioniert, müssen die auszuwertenden Daten in den Quellprogrammen identisch gepflegt werden. Beispielsweise müssen die Fächer (Fachkürzel) im Stundenplanprogramm und in der Schulverwaltung gleich sein.

Werden aus der Schulverwaltung Daten zu Schülern und Klassen, aber keine Fächerangaben, importiert und liegen in der Stundenplanung (DaVinci oder UNTIS) keine Schülerdaten vor, dann werden im Enbrea Klassenbuch keine Kurszuweisungen vorgenommen. Diese müssen Sie nach dem Erstimport einmalig im Enbrea Klassenbuch pro Klasse machen. Bitte gehen Sie dazu in die Ansicht Unterricht > Klassen > Schülerzuweisung zu Kursen.

Nutzen Sie Magellan, muss die Kurszuweisung im Enbrea Klassenbuch nicht nachgepflegt werden. Hier kommt diese Zugehörigkeit direkt aus Magellan (Voraussetzung: gleiche Fachkürzel).

## Kurswechsel in DaVinci¶

Kommt es in DaVinci zu einem Kurswechsel bei einem Schüler, ist wird der Schüler nach der Änderung und dem Übertrag nach Enbrea in beiden Kursen geführt.Das Zu- und Abgangsdatum beim Kurswechsel muss in Enbrea selbst geändert werden unter Kurse.

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

