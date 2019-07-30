# Lehrer-Zeitkonten

![](/assets/Lehrer-Soll-Konto.png)

Im Lehrer-Zeitkonto Fenster erfassen Sie für einen Lehrer dessen Ermäßigungs- und Mehrarbeitsstunden. Die Ermäßigungs- und Mehrarbeitsgründe können Sie im Schlüsselverzeichnis ``Extras >> Schlüsselverzeichnisse >> Lehrer-Soll-Schlüssel`` eingeben.

Für jeden Ermäßigungs- bzw. Mehrarbeitsgrund geben Sie in der Spalte „Stunden“ die entsprechende Stundenzahl ein.

Operator |	Beschreibung
---|---
P | Pflicht- oder Regelstunden, die einem Lehrer aufgrund rechtlicher Vorgaben als allgemeine Unterrichtsverpflichtung auferlegt sind. Geben Sie in der Spalte „Stunden“ die betreffende Stundenzahl an. Einen Standardwert können Sie unter ``Extras > Optionen > Einstellungen > Lehrer-Pflichtstunden standardmäßig`` eingeben.
- | Ermäßigungsstunden, um welche die allgemeine Unterrichtsverpflichtung des Lehrers gemindert wird. Geben Sie in der Spalte „Stunden“ die betreffende Stundenzahl an. 
+ | Ergänzungs- bzw. Mehrarbeitsstunden, um welche die allgemeine Unterrichtsverpflichtung des Lehrers erhöht wird
D | Differenz aus Soll und Ist vom Vorjahr. Die Stundenanzahl in der Spalte „Stunden“ wird beim Erstellen eines neuen Stundenplans über den Planvorbereitungsassistenten automatisch aus dem vorhergehenden Plan übernommen. Sie können sie hier auch manuell eingeben. Dieser Wert fließt nicht in die Berechnung ein, dient der Information.
A | Stundenplan-Zeitkonto: In der Ansicht ``Stammdaten > Fächer`` können Sie in der Spalte „Zeitkonto“ für einem Fach einen Lehrer-Soll-Schlüssel als Zeitkonto zuweisen. Die Stundenanzahl in der Spalte „Stunden“ wird in diesem Fall automatisch aufgrund des Lehrerplans berechnet. 
C | Kalender-Zeitkonto: In der Ansicht „Kalender“ können Sie im Ereignis-Fenster bei „Zeitkonto“ einem Ereignis einen Lehrer-Soll-Schlüssel als Zeitkonto zuweisen. Die Stundenanzahl in der Spalte „Stunden“ wird in diesem Fall automatisch aufgrund des der entsprechenden Klandereinträge berechnet. 
Leer | Bemerkung, geht nicht in die Berechnung ein
