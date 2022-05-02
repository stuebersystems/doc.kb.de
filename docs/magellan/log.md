# Logdatei bei einer Installation erzeugen

[1]:/assets/images/magellan/13.png "Ausführen aufrufen"
[2]:/assets/images/magellan/14.png "Ausführen"

Wenn bei einer Installation Probleme auftreten, kann die Logdatei der Installation hilfreich sein. Bitte erzeugen Sie die Logdatei nach folgender Anleitung und senden uns diese bitte zu.

1. Erstellen Sie unter `C:\` ein Verzeichnis `Installationspakete` auf dem Rechner, auf dem installiert werden soll.
2. Legen Sie in dieses Verzeichnis bitte das Installationspaket, im nachfolgenden Beispiel das "magellan9.msi", das Vorgehen für andere Programme (davinci6.msi usw.) ist identisch.
3. Erzeugen Sie in dem Verzeichnis bitte eine Textdatei mit dem Namen `log.txt`.
4. Klicken Sie unten links auf Start und rufen `Ausführen` auf!

[![Ausführen aufrufen][1]

5. Fügen Sie die nachfolgende Zeile ein und drücken auf OK!<br/>`msiexec /i C:\Installationspakete\magellan9.msi /l*v log.txt` 

[![Ausführen][2]

1. Bitte durchlaufen Sie die Schritte der Installation. 
2. Nach der Installation ist die `log.txt` gefüllt, bitte senden Sie diese Datei als Ticketanhang mit, vielen Dank!