# Verrechnungsarten

Die Verrechnungsart hat entscheidenen Einfluss auf die statistischen Summen, die von DAVINCI ermittelt werden und die dann an die Landesstatistik übermittelt werden.
Klassenfaktor, Lehrerfaktor und Periodenfaktor werden nur bei den Verrechnungsarten "faktorbezogen" und "wochenbezogen" berücksichtigt. Sie dienen dazu, den Unterricht, der nicht jede Woche gleich stattfindet, auf einen vergleichbaren Wochenmittelwert herunterzurechnen.
Da die meisten Schulen mit Wochensummen arbeiten, erfordert die Landesstatistik in den meisten Fällen faktorbezogene Summen. Zusammengefasst und die weiteren Erläuterungen vorweggenommen ergibt sich so folgende Regel:

* Wenn Sie überwiegend mit wöchentlichen Terminen planen, sollten Sie mit der Verrechnungsart "faktorbezogen" arbeiten
* Wenn Sie überwiegend mit einmaligen Terminen planen, sollten Sie mit der Verrechnungsart "tagesbezogen" arbeiten

## Verrechnungsart "faktorbezogen"

Nehmen wir als Beispiel den Unterricht 

	2 Stunden BWL in jeder geraden Woche
	
Die ergibt für das Wochenmittel 
	
	W = 2 Stunden x 0,5 = 1 Stunde
	
Der Faktor 0,5 ergibt sich, falls bei der "Veranstaltung > Zeitdetails" die Option Klassenfaktor "Automatisch berechnen" eingestellt wurde:

* falls die Option Klassenfaktor "Automatisch berechnen" nicht eingestellt wurde: 
  aus dem manuell eingegebenen Klassenfaktor bei "Veranstaltung > Zeitdetails" 
* falls die Option Klassenfaktor "Automatisch berechnen" eingestellt wurde:
  * aus dem Periodenfaktor, falls die Veranstaltung eine Periode hat oder
  * aus dem Quotienten aus Anzahl der Unterrichtswochen dieser Veranstaltung und dem Wochenfaktor (siehe "Plan > Einstellungen > Statistik > Wochenfaktor").
      Unterrichtswochen sind dabei die rechnerischen Wochen, die bei "Wochenbezogene Summen" unter "Plan > Einstellungen > Statistik" markiert wurden.	  


> Problematisch wird es bei dieser Verrechnungsart, wenn auch einmalige Termine verrechnet werden sollen. Bei der Unterrichtsplanung sind beispielsweise zusätzlich 10 Tage "Praxis" geplant.
Solange nicht klar ist, ob die 10 Termine über zwei oder mehrere Wochen verteilt stattfinden, kann kein Wochenmittel bestimmt werden. In diesem Fall muss auf "Automatisch berechnen" des Faktors verzichtet werden und stattdessen der entsprechende Faktor manuell eingegeben werden, z.B. 2/40 = 0,5 (falls Wochenfaktor = 40, siehe "Plan > Einstellungen > Statistik > Wochenfaktor").

## Verrechnungsart "wochenbezogen"

Diese Verrechnungsart unterscheidet sich von der vorhergehenden nur in der Berechnung des Faktors:

Der Faktor 0,5 ergibt sich, falls bei der "Veranstaltung > Zeitdetails" die Option Klassenfaktor "Automatisch berechnen" eingestellt wurde:

 * aus dem Periodenfaktor, falls die Veranstaltung eine Periode hat oder
 
 * aus dem Quotienten aus Anzahl der Unterrichtswochen dieser Veranstaltung und dem Wochenfaktor (siehe "Plan > Einstellungen > Statistik > Wochenfaktor"). Unterrichtswochen sind dabei die Wochen, die bei "Wochenbezogene Summen" unter "Plan > Einstellungen > Statistik" markiert wurden.	  

## Verrechnungsart "tagesbezogen"

Bei dieser Verrechnungsart spielen die Faktoren keine Rolle, hier wird der tatsächlich stattfindende bzw. der tatsächlich gehaltene Unterricht berechnet.

Nehmen wir als Beispiel den Unterricht 

	2 Stunden BWL in jeder geraden Woche
	
Der Unterricht findet in 40 von insgesamt 44 Unterrichtswochen (dem Wochenfaktor, siehe "Plan > Einstellungen > Statistik > Wochenfaktor") statt. 
Damit ergibt sich Stundensumme pro Jahr Y:

	Y = 2 Stunden BWL x 40 = 88 Stunden/Jahr
	
Daraus errechnet sich das rechnerische Wochenmittel W wie folgt:

	W = Y / 44 = 88 / 44 = 2 Stunden 

Nehmen wir an, eine der BWL Stunden findet in einer der Wochen aufgrund eines Feiertags (z.B. Gründonnerstag) nicht statt. Die Stundenanzahl pro Jahr reduziert sich damit von 88 auf 87. Dann errechnet sich das tatsächliche Wochenmittel W wie folgt:

	W = 87 / 44 = 87 / 44 = 1,977 Stunden 

> #### info::Hinweis
>
> Durch die mögliche Abweichung von rechnerischem Wochenmittel und tatsächlichem Wochenmittel	kann es zu einer Soll/Ist Differenz beim Lehrer kommen. Sind noch keine Stunden des BWL-Lehrers verplant, ist der Lehrer mit einem Soll von 2 Stunden pro Woche in der Unterrichtsplanung erfasst. Sobald die Stunden verplant sind, ist der tatsächliche Wert 1,977 Stunden. Um dieses Dilemma zu vermeiden, sollte man bei dieser Verrechnungsart daher grundsätzlich mit jahresbezogenen Summen arbeiten.

