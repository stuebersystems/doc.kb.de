# ODBC-Anbindung unter Windows 64 bit

!!! danger "Wichtig!"

    Dieser Hinweis ist nur bis Version 7 von MAGELLAN relevant. 
    Jüngere MAGELLAN-Versionen gibt es in 32 oder 64 Bit Ausgabe. Der Unterschied bezieht sich nicht MAGELLAN selbst (immer 32 Bit), sondern die ODBC Anbindung, die für den Druck  und die Druckvorschau aus MAGELLAN heraus verwendet wird. Das hat auch nichts mit dem Druck oder der Vorschau aus MAGELLAN heraus zu tun, der Druck würde auch funktionieren, wenn Sie auf einem 64 Bit Betriebssystem die 32 Bit MAGELLAN-Version installieren würden.
    Es geht um Folgendes: Die Vollversion von Crystal Reports, die man benötigt um selbst Berichte anzupassen, gibt es nur noch in 64 Bit. Für Schulen, die Crystal Reports zum Ändern einsetzen, richten wir mit der 64 Bit-MAGELLAN.msi die passende ODBC-Anbindung ein.

Mit der Installation von MAGELLAN wird für 32 Bit Betriebssysteme bereits eine ODBC-Anbindung eingerichtet, die Sie für den Zugriff des Reportgenerators Crystal Reports auf die MAGELLAN-Datenbank verwenden können. Für 64 Bit Betriebssysteme kann es sein, dass diese Anbindung manuell eingerichtet werden muss. 

Bitte führen Sie folgende Schritte aus:

1. Deinstallieren Sie auf diesem Rechner bitte Ihre Firebird-Version und auch MAGELLAN.

2. Löschen Sie anschließend den Verzeichnissen System, System32 und auch SysWOW64  die eventuell noch vorhandenen Dateien: `ODBCJDBC.dll` und `ODBCJDBCinst.dll`.

3. Installieren Sie anschließend den von uns zur Verfügung gestellten Firebird-Treiber mit den Standardvorgaben plus dem Häkchen, wie im nachstehenden Screenshot:  
  
  ![Einstellungen im Firebird Setup](/assets/images/fb-inst.jpg)

4. Installieren Sie [MAGELLAN] erneut. Hier finden Sie die [Installationsanleitung].

5. Prüfen Sie anschließend im Verzeichnis `SysWOW64`, ob die Dateien `ODBCJDBC.dll` und `ODBCJDBCinst.dll` vorhanden sind. Falls nicht, kopieren Sie diese aus dem Verzeichnis `System32` dorthin. 

6. Öffnen Sie nun das das Verzeichnis `SysWOW64` und starten die Anwendung `ODBCAD32.exe`. Bitte richten Sie hier die ODBC-Anbindung analog dem nachstehenden Screenshot ein (der Datenbankpfad ist nur ein Beispiel und muss angepasst werden):  
  
  ![Firebird ODBC Setup](/assets/images/fb-odbc.png)

[MAGELLAN]: http://magellan.stueber.de/download.php
[Installationsanleitung]: https://doc.magellan.stueber.de/installation