# Importlogik MAGELLAN und DAVINCI

## Kurszuordnung in ENBREA 

Unter `Stammdaten > Kurse` werden die Schüler je Kurs gezeigt. Dabei werden je nach eingesetzten Quellprogrammen (Schulverwaltung und Stundenplanung) Daten ausgewertet und die Schüler-Kurszugehörigkeit rückgeschlossen.

Damit das Rückschließen auf die Schüler je Kurs funktioniert, müssen die auszuwertenden Daten in den Quellprogrammen identisch gepflegt werden. Beispielsweise müssen die Fächer (Fachkürzel) im Stundenplanprogramm und in der Schulverwaltung gleich sein.

Werden aus der Schulverwaltung Daten zu Schülern und Klassen, aber keine Fächerangaben, importiert und liegen in der Stundenplanung (DAVINCI oder UNTIS) keine Schülerdaten vor, dann werden im ENBREA Klassenbuch keine Kurszuweisungen vorgenommen. Diese müssen Sie nach dem Erstimport einmalig im ENBREA Klassenbuch pro Klasse machen. Bitte gehen Sie dazu in die Ansicht Unterricht > Klassen > Schülerzuweisung zu Kursen.

Nutzen Sie MAGELLAN, muss die Kurszuweisung im ENBREA Klassenbuch nicht nachgepflegt werden. Hier kommt diese Zugehörigkeit direkt aus MAGELLAN (Voraussetzung: gleiche Fachkürzel).

## Kurswechsel in DAVINCI¶

Kommt es in DAVINCI zu einem Kurswechsel bei einem Schüler, ist wird der Schüler nach der Änderung und dem Übertrag nach ENBREA in beiden Kursen geführt.Das Zu- und Abgangsdatum beim Kurswechsel muss in ENBREA selbt geändert werden unter Kurse

## Neues Schuljahr¶

Arbeiten Sie nur mit dem Stundenplanprogram DAVINCI und verwalten dort auch Ihre Schüler achten sie bitte unbedingt darauf zu Beginn eines neuen Schuljahres die Klassenzugehörigkeit der Schüler in DAVINCI zu ändern Stammdaten > Schüler > Klasse.

## Schüler in mehreren Klassen¶

Schüler werden anhand der Information zu Vorname, Nachname, Geburtsdatum geprüft. Ist ein Schüler in DAVINCI > Stammdaten > Schüler doppelt angelegt und unterscheidet sich nur in der DAVINCI > Stammdaten > Schüler > Klasse wird der Schüler nur einmal in den ENBREA Stammdaten angelegt, aber beiden Klassen als Schüler zugeordnet.
Nebenlaufbahn eines Schülers¶

Hat eine Schüler in MAGELLAN in MAGELLAN eine Haupt- und Nebenlaufbahn Schüler > Auswahl > Laufbahn > H/N wird diese durch Klassenzugehörigkeit zu beiden Klassen in ENBREA mit den jeweiligen Zu- und Angangsdaten berücksichtigt.

## Fächer in MAGELLAN und DAVINCI

In der Regel haben Sie in DAVINCI keine Schüler und Schülerinnen den Unterrichtsveranstaltungen zugewiesen. In MAGELLAN haben die Schüler und Schülerinnen aber unter `Schüler > Zeugnis > Fächer` ihre zugewiesenen Fächer. Achten Sie darauf, dass Sie MAGELLAN und DAVINCI die gleichen Fachkürzel verwenden. In diesem werden werden die Schüler und Schülerinnen automatisch beim Datenimport nach ENBREA Klassenbuch den entsprechenden Kursen zugewiesen.

## Fach in DAVINCI aber nicht in MAGELLAN

In der Regel haben Sie in DAVINCI keine Schüler und Schülerinnen den Unterrichtsveranstaltungen zugewiesen. Wurde dem Schüler oder der  Schülerin in MAGELLAN unter `Schüler > Zeugnis > Fächer` ein Fach nicht zugewiesen, kann beim Datenimport nach ENBREA Klassenbuch den entsprechenden Kursen kein Schüler oder Schülerin zugewiesen werden. Sie können in diesem Fall im ENBREA Klassenbuch `Stammdaten > Kurse > Schülerzuweisung zu Kursen` machen. In diesem Fall werden alle Schülerinnen und Schüler der Klasse zugewiesen.

## Fach in DAVINCI mit Gruppenteilung

Haben Sie ein Fach, welches in Teilung also in mehreren Gruppen unterrichtet wird, empfiehlt es sich, hier in DAVINCI in MAGELLAN die Fächer als Kurse also mit Kursnummern anzulegen. Durch die Zuordnung der Fächer mit Kursnummer in MAGELLAN ensteht die Kurszuordnung der Schülerinnen und Schüler. Alternativ können Sie auch in DAVINCI Schülerinnen oder Schüler der Veranstaltung zuweisen, dazu müssen aber in den `Stammdaten > Schüler` hinterlegt sein.

## Fächer in der gymnasialen Oberstufe

In der gymnasialen Oberstufe werden die Kursbildungen im DAVINCI Kursplan gemacht. Das heißt hier werden die Zuordnungen der Schülerinnen und Schüler in DAVINCI gemacht und automatisch beim Datenimport nach ENBREA Klassenbuch den entsprechenden Kursen zugewiesen.

## Emailadressen in MAGELLAN und DAVINCI

Haben Sie für Ihre Lehrkräfte in MAGELLAN und DAVINCI Emailadressen hinterlegt, die von einander abweichen, wird beim ersten Import nach der Importreihenfolge gegangen. Also gegebenefalls erst die Emailadresse aus DAVINCI hinterlegt und dann geändert mit der in MAGELLAN hinterlegten Emailadresse.

## Klassenwechsel in MAGELLAN

## Ausschulen in MAGELLAN

