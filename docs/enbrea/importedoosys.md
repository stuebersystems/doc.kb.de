# Importlogik edoosys

Schüler_Stamm_ID: Definiert einen Schüerldatensatz	
Vornamen: Vorname des Schülers	
Familienname: Nachname des Schülers	
Geburtsdatum: Geburtsdatum des Schülers		
Geschlecht (männlich/weiblich).Kurzform: Geschlecht des des Schülers	
Klasse / Klassengruppe: Klassengruppe	
Klasse: Klasse
Alle Lehrkräfte (Kürzel) mit Fach: Kurszugehörigkeit des Schülers; Kurs definiert sich aus dem Fach und der Lehrkraft in einer Klasse. 

!!! info "Achtung"

    Beim Import nach Enbrea kann angegeben werden, ob die Klassengruppen berücksichtigt werden sollen. Beim Einsatz von edoo.sys UND DaVinci hängt die Einstellung davon ab, ob in DaVinci mit Klassengruppen oder nur mit Klassen geplant wird. Die exportierten Klassendaten aus DaVinci und edoo.sys müssen übereinstimmen.

!!! info "Achtung"

    Achten Sie bei der Arbeit mit DaVinci darauf, dass die KLassekürzel, Kürzel der Lehrkräfte und Fächer mit denen aus edoosys übereinstimmen müssen.

## Neue Schüler im Schuljahr

Die Schüler werden nach Enbrea in die `Stammdaten > Schüler`, `Stammdaten > Klasse` und `Stammdaten > Kurse` übernommen. Das Zugangsdatum bei den Kursen muss in Enbrea selbst geändert werden unter `Stammdaten > Kurse`. Das heisst, durch den Import wird kein späteres Zugangsdatum zugewiesen. Die Kurszugehörigkeit entspricht erstaml immer der Gültigkeitsdauer des Kurses. 

## Schüler haben die Schule verlassen

Tauchen Schüler nicht mehr in der export.csv aus edoosys auf, wird die Klassenzugehörigkeit der Schüler in den `Stammdaten > Schüler` gelöscht.
In `Stammdaten > Klasse` wird der Schüler nicht angezeigt.

Das Abgangsdatum bei den Kursen muss in Enbrea selbst geändert werden unter `Stammdaten > Kurse`. Das heisst, durch den Import wird keine Schüler aus den Kursen gelöscht. Dies kann, wenn benötigt nur direkt in Enbrea gemacht werden. 

## Klassenwechsel von Schülern

Bei einem Wechsel der Klasse sind die Schüler in der neuen Klasse und den neuen Kursen vermerkt. Das Abgangsdatum bei den alten Kursen muss in Enbrea selbst geändert werden unter `Stammdaten > Kurse`. Das heisst, durch den Import wird keine Schüler aus den Kursen gelöscht. Dies kann, wenn benötigt nur direkt in Enbrea gemacht werden. Das Zugangsdatum bei den neuen Kursen muss in Enbrea selbst geändert werden unter `Stammdaten > Kurse`. 

## Kurswechsel von Schülern

Insofern der "neue Kurs" in Enbrea existiert, wird der Schüler nach Enbrea in die `Stammdaten > Kurse` übernommen. Das Zugangsdatum bei den Kursen muss in Enbrea selbst geändert werden unter `Stammdaten > Kurse`. Das heisst, durch den Import wird kein späteres Zugangsdatum zugewiesen. Die Kurszugehörgkeit entspricht erstaml immer der Gültigkeitsdauer des Kurses. 

## Änderung von Schülerstammdaten

Die Identifikation des Schülers erfolgt anhand der Schüler_Stamm_ID. Das heisst, geänderter Vorname, Nachname oder Geburtsdatum bei gleicher Stamm Id werden nach Enbrea übertragen. Der bestehende Schülerdatensatz wird geändert.

