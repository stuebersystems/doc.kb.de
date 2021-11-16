# Sorgeberechtigte für Nebenschüler anzeigen

Um für Nebenschüler die Sorgeberechtigen auszugeben, müssen Sie in Ihren Berichten die nachstehende Änderunge vornehmen.

Wechseln Sie in den Feldexplorer und legen eine neue Formel an.

![neue Formel](/images/cr/10.png)

Vergeben Sie bitte einen Formelnamen, in unseren Berichten heißt die Formel `SchuelerID`.

![neue Formel](/images/cr/15.png)

Öffnen Sie die neue Formel per Doppelklick und fügen den nachfolgenden Formeltext ein, speichern Sie die Formel.

```
if not IsNull({Schueler.IDIntern}) then 
  formula = {Schueler.IDIntern}
else
  formula = {Schueler.ID}
end if
```

!!! info "Hinweis"

    Die Formel prüft den Inhalt des Feldes `SchuelerID.Intern`.

    Ist das Feld leer, wird die SchuelerID benutzt,es handelt sich also um einen `Stammschüler`. 

    Ist das Feld nicht leer, wird der Inhalt genutzt, es handelt sich um einen `Nebenschüler`.

![neue Formel](/images/cr/16.png)

Jetzt muss die Formel noch mit dem Unterbericht mit den Sorgeberechtigtendaten verknüpft werden. Klicken Sie mit rechter Maustaste auf den Unterbericht und wählen `Unterberichtsverknüpfungen ändern`.

![neue Formel](/images/cr/09.png)

Markieren Sie in der rechten Fensterhälfte `AuswahlSchueler.Schueler` und setzen ihn per Pfeil nach links zurück in die Auswahlliste.

![neue Formel](/images/cr/11.png)

Suchen Sie in der rechten Fensterhälfte die Formel `SchuelerID` und übergeben sie per Pfeil nach rechts in die `Felder für Verknüpfung`.

![neue Formel](/images/cr/12.png)

Prüfen Sie die Feldverknüpfungen entsprechend der folgenden beiden Abbildungen:

![neue Formel](/images/cr/13.png)

![neue Formel](/images/cr/14.png)

Fertig!