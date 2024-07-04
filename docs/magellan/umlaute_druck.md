# Magellan [7/8]: In der Druckvorschau werden Umlaute nicht richtig dargestellt

Beim Aufruf der Druckvorschau stellt Magellan seine gewünschten Einstellungen in der ODBC-Anbindung (`Systemsteuerung > Verwaltung > ODBC 32Bit`) ein oder legt diese auch ggfs. neu an.
Als Zeichensatz möchte Magellan gern UTF8 einstellen. Das muss in der Liste aber auch vorhanden sein.

> Wichtig ist, dass der Eintrag nicht nur im Feld sichtbar ist, sondern auch in der Liste hinter diesem Feld auswählbar ist! Bei Rechnern, auf denen dieser Eintrag in der Liste fehlt, muss bitte der Treiber aktualisiert werden.

![Hier ist der Eintrag korrekt in der Liste vorhanden](/assets/images/odbc_umlaute.png)

Downloadseite|Eintrag
--|--
https://firebirdsql.org/en/odbc-driver/ | Windows 32-bit Full Install

Magellan bitte schließen, das Paket laden und die Installation ausführen.
Anschließend bitte Magellan neu starten, die Umlaute sollten im Druck jetzt korrekt dargestellt werden.
