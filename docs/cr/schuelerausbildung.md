# Änderung in der Tabelle SchuelerAusbildung

Mit der Magellan-Ausgabe 6.0.68 gab es eine Änderung in der Tabelle `SchuelerAusbildung`. Unsere Berichte haben wir dahingehend angepasst und per Service-Update veröffentlicht. 

Bitte beachten Sie für Ihre eigenen Berichte, dass in der Tabelle `SchuelerAusbildung` statt des Feldes `Ausbilder` jetzt das Feld `AusbilderKontakt` existiert, das auf die Tabelle `BetriebeKontakte` verweist.

Sollte Ihnen der Feldexplorer in Crystal Reports noch das Feld `Ausbilder` zeigen, dann passiert es, weil es zum Zeitpunkt als der Bericht erstellt wurde, dieser Stand aktuell war.

Bitte entfernen Sie die Tabelle aus Ihrem Bericht, fügen sie wieder neu ein und setzen die Verknüpfungen wieder wie zuvor.

Die Datenstrukturbeschreibung für Magellan 6 finden Sie unter [https://doc.magellan6-ds.stueber.de/](https://doc.magellan6-ds.stueber.de/)
Die Datenstrukturbeschreibung für Magellan finden Sie unter [https://doc.magellan-toolbox.stueber.de/datenstruktur/](https://doc.magellan-toolbox.stueber.de/datenstruktur/).