# Empfohlene Verknüpfungen

## Schülerberichte

![Beispiel für einen Schülerbericht](/images/cr/05.png)

Tabelle|Tabelle|anschließende Tabellen
--|--|--
**SchuelerZeitraeume**<br/>Mandant =><br/>Schueler =>|**Schueler**<br/>Mandant<br/>ID|--
**SchuelerZeitraeume**<br/>Mandant =><br/>ID =>|**SchuelerFachdaten**<br/>Mandant<br/>SchuelerZeitraumID|Beispiel: Noten, Faecher...
**SchuelerZeitraeume**<br/>Mandant =><br/>Ausbildung =>|**SchuelerAusbildung**<br/>Mandant<br/>ID|Beispiel: Beruf...<br/> Wichtig: Bitte die Verknüpfungen zwischen der Tabelle Schueler und Tabelle SchuelerAusbildungen aufheben
**SchuelerZeitraeume**<br/>Mandant =><br/>KlassenZeitraumID =>|**Klassenzeitraeume**<br/>Mandant<br/>ID|Beispiel: Klassen, Lehrer...
**SchuelerZeitraeume**<br/>Mandant =><br/>ID =>|**SchuelerKlassen**<br/>Mandant<br/>SchuelerZeitraumID|--
**Schueler**<br/>Mandant =><br/>ID =>|**SchuelerFoerderungen**<br/>Mandant<br/>Schueler|Beispiel: Behinderungsart<br/>Wichtig: Bitte im Detailbereich verwenden oder einen Unterbericht nutzen, das Ergebnis ist eine Liste von Werten
**Schueler**<br/>Mandant =><br/>ID =>|**SchuelerSorgeberechtigte**<br/>Mandant<br/>Schueler|Beispiel: Sorgeberechtigte
**SchuelerZeitraeume**<br/>Mandant =><br/>ID =>|**SchuelerZeugnisbemerkungen**<br/>Mandant<br/>SchuelerZeitraumID|--

## Klassenberichte

![Beispiel für einen Klassenbericht](/images/cr/08.png)

Tabelle|Tabelle|anschließende Tabellen
:--|:--|:--
**KlassenZeitraeume**<br/>Mandant =><br/>ID =>|**SchuelerZeitraeume**<br/>Mandant<br/>KlassenZeitraumID|Beispiel:<br/>SchuelerZeugnisbemerkungen<br/>Mandant => Mandant<br/>ID => SchuelerZeitraumID