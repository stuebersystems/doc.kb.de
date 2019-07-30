# Berechnungskonzepte in daVinci

In daVinci 6 stehen drei verschiedene Berechnungskonzepte zur Verfügung, die Sie für die Ermittlung der Stundensummen benutzen können: 

*	Faktorbezogene Berechnung 
*	Wochenbezogene Berechnung 
*	Tagesbezogene Berechnung 

Je nachdem wofür bzw. in welcher Genauigkeit Sie die Daten benötigen, können Sie die Stundensummen unterschiedlich berechnen lassen. Jedes der drei Berechnungskonzepte berücksichtigt unterschiedliche Informationen in der Plandatei und führt zu unterschiedlichen Ergebnissen. Die Unterschiede beziehen sich dabei auf die Summen-Kategorien: „Lehrer-Ist“, „Lehrer-Ist in Klasse“ und „Schüler-Ist“.


Verrechnungsart|	Beschreibung
---|---
**Tagesbezogen**|	Es wird jeden Tag die Anzahl der Stunden gezählt, wobei unterrichtsfreie Tage laut Kalender wie z.B. Ferien und Feiertage nicht mitgezählt werden. Das Resultat ist eine genaue Stundensumme über die Wochen und das Schuljahr, z.B. „2h je Woche in 20 Wochen des Schuljahres = 2h x 20 = 40h [im Schuljahr] => 40h / 40 Wochen = 1h/Woche [als Wochenmittelwert]“.
**Wochenbezogen**|	Es wird jeden Tag die Anzahl der Stunden gezählt, wobei die in „Wochenbezogene Summe“ ausgenommenen Wochen nicht mitgezählt werden. Das Resultat ist eine gemittelte Stundensumme über die Wochen des Schuljahres, z.B. „2h x 20 Wochen / 40 Wochen = 1h [je Woche als Mittelwert]“
**Faktorbezogen**|	Die jeweilige Stundendauer einer Veranstaltung wird mit dem Klassenfaktor (aus Klassensicht) bzw. dem Lehrerfaktor (bei Lehrersicht) multipliziert. Klassenfaktor und Lehrerfaktor können je Veranstaltung über das Dialogfenster „Veranstaltung“ manuell eingegeben werden oder errechnen sich automatisch aus dem Faktor der ggf. zugewiesenen Periode.

##	Faktorbezogene Berechnung

Bei diesem Berechnungskonzept werden die Wochendurchschnitts- und Jahresstundenwerte der genannten Summenkategorien auf der Basis wochenbezogener Berechnungsfaktoren gebildet. Alle Werte werden nur aufgrund der im Teilfenster „Veranstaltungsliste“ vorhandenen Terminformationen ermittelt. Informationen über Ferien und Feiertage und andere schulfreie Ereignisse, die nur im Teilfenster „Planungsfenster“ vorhanden sind, werden nicht berücksichtigt.

Bei der faktorbezogenen Berechnung fließen folgende Informationen in die Berechnung der Stundensummen ein: 

*	Die Angaben in der Spalte „Dauer/W“ der Veranstaltungsliste 
*	Der individuelle Klassenfaktor der Veranstaltungen. 
*	Der individuelle Lehrerfaktor der Veranstaltungen. 
*	Der allgemeine Wochenfaktor in den Statistikeigenschaften der Datei. 
*	Die Informationen über die ausgenommenen Wochen in den Statistikeigenschaften der Datei. 
*	Die Angaben in der Spalte „Block“ der Veranstaltungsliste 
*	Die Angaben in der Spalte „Wochen“ der Veranstaltungsliste

##	Wochenbezogene Berechnung

Bei der wochenbezogenen Berechnungsweise werden die Stundenwerte der Lehrer und Klassen in den vom Planer definierten Unterrichtswochen zu Jahresstundenwerten addiert. Die zugehörigen Durchschnittswerte ergeben sich, indem die Jahresstundenwerte durch den allgemeinen Wochenfaktor in den Statistikeigenschaften der Datei dividiert werden. Zur Ermittlung der Ist-Stundenwerte werden nur die im Teilfenster „Veranstaltungsliste“ verfügbaren Termininformationen herangezogen. Informationen über Ferien- und Feiertage und andere schulfreie Ereignisse, die nur im Teilfenster „Planungsfenster“ hinterlegt sind, werden nicht berücksichtigt. Allerdings wird berücksichtigt, wenn gesetzte Termine sich im Plan überschneiden z.B. aufgrund von Schienen.

Bei der wochenbezogenen Berechnung fließen folgende Informationen in die Berechnung der Stundensummen ein: 

*	Die Angaben in der Spalte „Dauer/W“ der Veranstaltungsliste 
*	Der allgemeine Wochenfaktor in den Statistikeigenschaften der Datei. 
*	Die Informationen über die ausgenommenen Wochen in den Statistikeigenschaften der Datei. 
*	Die Angaben in der Spalte „Block“ der Veranstaltungsliste 
*	Die Angaben in der Spalte „Wochen“ der Veranstaltungsliste 
*	Die Angaben in der Spalte „Zeit“ der Terminzeilen in der Veranstaltungsliste

##	Tagesbezogene Berechnung

Bei der tagesbezogenen Berechnung werden die Lehrer-Ist-Werte für die einzelne Unterrichtswoche ermittelt, indem die Dauer der im Teilfenster „Planungsfenster“ definierten Unterrichtstermine miteinander addiert werden. Informationen über unterrichtsfreie Ereignisse, wie z.B. Ferien oder Feiertage werden dabei berücksichtigt. Der Jahresstundenwert des Lehrer-Ist wird errechnet, indem die Stundenwerte der einzelnen Wochen miteinander addiert werden. Der Wochendurchschnittswert des Lehrer-Ist wird gebildet, indem der Jahresstundenwert durch einen automatisch generierten Wochenfaktor dividiert wird.

Bei der tagesbezogenen Berechnung fließen folgende Informationen in die Berechnung der Stundensummen ein: 

*	Anfangs- und Enddatum des Planungszeitraums 
*	Unterrichtsfreie Termine 
*	Dauer der Unterrichtstermine 
*	Überschneidungsinformationen im Planungsfenster 
*	Automatisch generierter Wochenfaktor 
