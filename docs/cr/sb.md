# Bewerberberichte mit Sorgeberechtigtendaten

[1]:/assets/images/cr/18.png "Datenbank-Assistent > SchuelerFamilie"
[2]:/assets/images/cr/19.png "Formel BewerberID"
[3]:/assets/images/cr/20.png "Unterberichtsverknüpfung mit Formel"

Problem:
Berichte, die für den Bewerber auch Sorgeberechtigtendaten ausgeben sollen, berücksichtigen nicht gesondert Schülerkopien.

Zur Erläuterung:
Eine Schülerkopie kann angelegt werden, um Schüler parallel in mehr als einer Klasse zu verwalten oder um aktuelle oder ehemalige Schüler im Bewerbermenü zu verwalten. Die Kopien sind nicht losgelöst vom "Urschüler" (Stammschüler) zu betrachten, viele Daten werden für die Schülerkopie vom  sind, werden vom Stammschüler eingeblendet. 
Insofern müssten zur Ausgabe der Sorgeberechtigtendaten eines kopierten Schülers nicht die Sorgeberechtigtendaten der Schülerkopie abgefragt werden, sondern die des Stammschülers. 

Am Beispiel des Berichts `Bewerberpersonalblatt`:

Der Bericht soll im Unterbericht "Eltern.rpt" die Sorgeberechtigtendaten ausgeben.
Dafür wurde der View "SchuelerFamilie" verwendet, hier sind alle nötigen Felder gesammelt enthalten.

[![Datenbank-Assistent > SchuelerFamilie][1]

Um für nicht kopierte Bewerber die Sorgeberechtigtendaten zur BewerberID und für die kopierten Bewerber die Sorgeberechtigtendaten des Datensatzes aus dem Feld IDIntern (enthält die ID des Stammschülers) auszugeben, wird für die Verknüpfung des Unterberichts eine Formel verwendet.

```
formula = {Schueler.ID}

if not IsNull({Schueler.IDIntern}) then 
  formula = {Schueler.IDIntern}
end if
```

[![Formel BewerberID][2]

Diese Formel wird in der Verknüpfung verwendet:

[![Unterberichtsverknüpfung mit Formel][3]




