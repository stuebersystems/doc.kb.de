# Barcodes formatieren

In Magellan gibt es einen Barcode für Schülerausweise und einen für Bibliotheksausweise. Für beide Felder gilt, dass für Berichte lediglich die Felder im Bericht verwendet werden und mit einer Schriftart formatiert werden, die dann aus der in der Datenbank gespeicherten Zeichenfolge einen Barcode für die Druckvorschau machen.

Bereich |Tabelle.Feld |Schriftart
--|--|--
`Magellan > Schüler`|Schueler.BarcodePrint| Code EAN 13
`Bibliothek > Ausleiher` |MedienAusleiher.BarcodePrint| Code 128