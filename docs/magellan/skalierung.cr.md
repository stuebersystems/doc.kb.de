# Darstellung exportierter PDFs

Die Darstellung von aus Crystal Reports exportierten PDFs und denen die mit Hilfe der Runtimeversion von Crystal Reports aus Magellan erzeugten PDFs weicht von einander ab.
Dieses Problem besteht innerhalb der Runtimeversion von Crystal Reports und kann nicht durch Magellan beeinflusst werden.

Im Internet wird ein Workaround beschrieben, bei dem zwei zusätzliche Registrywerte je Arbeitsplatz gesetzt werden (insgesamt an zwei Stellen, zweiter Pfad ist unter den Abbildungen).

Stellen zum Ändern des Schlüssels:

```HKEY_CURRENT_USER\SOFTWARE\SAP BusinessObjects\Suite XI 4.0\Crystal Reports\Export\PDF```

```HKEY_CURRENT_USER\SOFTWARE\SAP BusinessObjects\Crystal Reports für .NET Framework 4.0\Crystal Reports\Export\PDF```

Hier ein Beispiel für das Anlegen des Schlüssels`ForceLargerFonts` mit dem Wert `1`. Gehen Sie wie folgt vor:

Öffnen Sie den Registrierungseditor Ihres Arbeitsplatzes und wechseln auf den ersten der oben genannten Pfade:

Klicken Sie jeweils auf der rechten Seite auf eine freie Stelle mit der rechten Maustaste und wählen `Neu > Zeichenfolge`.

![](/assets/images/magellan/02.png)

Benennen Sie den neuen Wert um in `ForceLargerFonts` und tragen als Wert bitte `1` ein.

![](/assets/images/magellan/03.png)

![Schlüssel ist eingetragen](/assets/images/magellan/01.png)

Wiederholen Sie die Schritte bitte für die zweite Stelle.