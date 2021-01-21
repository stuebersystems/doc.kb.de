# Darstellung exportierter PDFs

Die Darstellung von aus Crystal Reports exportierten PDFs und denen die mit Hilfe der Runtimeversion von Crystal Reports aus MAGELLAN erzeugten PDFs weicht von einander ab.
Dieses Problem besteht innerhalb der Runtimeversion von Crystal Reports und kann nicht durch MAGELLAN beeinflusst werden.

Im Internet wird ein Workaround beschrieben, bei dem ein zusätzlicher Registrywert je Arbeitsplatz gesetzt wird.

So gehen Sie vor:

Öffnen Sie den Registrierungseditor Ihres Arbeitsplatzes und wechseln auf:

``Computer\HKEY_CURRENT_USER\SOFTWARE\SAP BusinessObjects\Crystal Reports for .NET Framework 4.0\Crystal Reports\Export
``

Klicken Sie auf der rechten Seite auf eine freie Stelle mit der rechten Maustaste und wählen `Neu > Zeichenfolge`.

![](/images/magellan/02.png)

Benennen Sie den neuen Wert um in `ForceLargerFonts` und tragen als Wert bitte `1` ein.

![](/images/magellan/03.png)

![Schlüssel ist eingetragen](/images/magellan/01.png)
