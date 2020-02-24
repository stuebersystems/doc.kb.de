# Empfohlene Verknüpfungen

![Beispiel für Verknüpfungen](/images/cr/05.png)

Tabelle|Tabelle|anschließende Tabellen
--|--|--
**SchuelerZeitraeume**<br/>Mandant<br/>Schueler|**Schueler**<br/>Mandant<br/>ID|--
**SchuelerZeitraeume**<br/>Mandant<br/>ID|**SchuelerFachdaten**<br/>Mandant<br/>SchuelerZeitraumID|Beispiel: Noten, Faecher...
**SchuelerZeitraeume**<br/>Mandant<br/>Ausbildung|**SchuelerAusbildung**<br/>Mandant<br/>ID|Beispiel: Beruf...<br/> Wichtig: Bitte die Verknüpfungen zwischen der Tabelle Schueler und Tabelle SchuelerAusbildungen aufheben
**SchuelerZeitraeume**<br/>Mandant<br/>KlassenZeitraumID|**Klassenzeitraeume**<br/>Mandant<br/>ID|Beispiel: Klassen, Lehrer...
**SchuelerZeitraeume**<br/>Mandant<br/>ID|**SchuelerKlassen**<br/>Mandant<br/>SchuelerZeitraumID|--