# Es werden mehr als die ausgewählten Datensätze gezeigt

Problem: Sie wählen in MAGELLAN nur wenige Datensätze aus um die Auswahltabellen zu füllen (`Drucken > Vorschau`), in der Crystal Reportsvorschau werden aber dennoch immer alle Datensätze aufgerufen.

Eine mögliche Ursache kann folgender Punkt sein:

CR optimiert vor dem Aufruf des Berichtes selbständig (und nicht unterdrückbar) die Abfrage. Gerade bei sehr einfachen Berichten kann das eigenständige Optimieren zu merkwürdigen Nebeneffekten führen. Was hilft, ist ein Feld (wir verwenden das Feld`Benutzer` aus der verwendeten Auswahltabelle) im oberen Bereich des Berichtes einzufügen und dann zu unterdrücken.

![Feld einfügen und ausblenden](/assets/images/cr/06.png)