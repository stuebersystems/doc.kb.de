# Drucksortierung der Datensätze in Berichten

## Problem

Man markiert in MAGELLAN ein Reihe von Datensätzen (Alfons, Bärbel und Cäsar) und ruft einen Bericht auf, die Anzeige der gefüllten Berichte ist nicht in der gewünschten Reihenfolge, sondern beispielsweise nach der ID.

## Lösung

1. Im Bericht eine neue Formel anlegen und benennen.

![neue Formel anlegen](/assets/images/cr/00.png)

2. In der Formel werden nacheinander die Sortierkriterien angegeben, jeweils getrennt durch `&`, als letztes Sortierkriterium kommt die ID, damit es eindeutig sortierbar ist.

Beispiel:

`formula = {Schueler.Nachname}&{Schueler.Vorname}&{Schueler.ID}`

![Felder und Operatoren angeben](/assets/images/cr/01.png)

3. Die Richtigkeit der Formel kann geprüft werden, anschließend speichern und schließen.

![Prüfen](/assets/images/cr/02.png)

4. Jetzt muss die Formel genutzt werden. Dafür links vor den Gruppenkopf in den graublauen Bereich klicken, linke Maustaste und `Gruppe wechseln` wählen.

!["Gruppe wechseln" aufrufen](/assets/images/cr/03.png)

5. Formel auswählen und den Haken vor der Option "Formel als Gruppensortierreihenfolge verwenden" aktivieren. Fertig!

!["Gruppe wechseln" aufrufen](/assets/images/cr/04.png)
