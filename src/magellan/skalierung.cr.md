# Darstellung exportierter PDFs

Die Darstellung von aus Crystal Reports exportierten PDFs und denen die mit Hilfe der Runtimeversion von Crystal Reports aus MAGELLAN erzeugten PDFs weicht von einander ab.
Dieses Problem besteht innerhalb der Runtimeversion von Crystal Reports und kann nicht durch MAGELLAN beeinflusst werden.

Im Internet wird ein Workaround beschrieben, bei dem zwei zusätzliche Registrywerte je Arbeitsplatz gesetzt werden (insgesamt an zwei Stellen).

So gehen Sie vor:

Öffnen Sie den Registrierungseditor Ihres Arbeitsplatzes und wechseln auf:

```
HKEY_CURRENT_USER\SOFTWARE\SAP BusinessObjects\Suite XI 4.0\Crystal Reports\Export\PDF
```

Klicken Sie jeweils auf der rechten Seite auf eine freie Stelle mit der rechten Maustaste und wählen `Neu > Zeichenfolge`.

![](/images/magellan/02.png)

Benennen Sie den neuen Wert um in `ForceLargerFonts` und tragen als Wert bitte `1` ein.

![](/images/magellan/03.png)

![Schlüssel ist eingetragen](/images/magellan/01.png)

Wiederholen Sie die Schritte bitte für:

```
HKEY_CURRENT_USER\SOFTWARE\SAP BusinessObjects\Crystal Reports für .NET Framework 4.0\Crystal Reports\Export\PDF
```
