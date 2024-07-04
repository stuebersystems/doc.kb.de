# Datenaustausch mit Sdui

## Fehlermeldungen beim Ausführen des Powershellskriptes

Fehler|Bedeutung
-|-
[Error] [Sdui] Bad Request:| Bitte überprüfen Sie die in der json.Datei eingetragene Sdui PIN
[Error] Local DaVinci file does not exist: |Bitte überprüfen Sie den in der json.Datei eingetragenen Dateinamen/Dateipfad der DaVinci Datei
[Error] Login konnte nicht erfolgreich ausgeführt werden. Möglicherweise ist der Benutzername oder das Kennwort falsch: |Bitte überprüfen Sie den in der json.Datei eingetragenen Benutzernamen und/oder das Kennwort
[Error] Socketfehler (Fehlercode: 10061).Connection refused: |Bitte überprüfen Sie den in der json.Datei eingetragenen Port.
[Error] Socketfehler (Fehlercode: 10051).Network is unreachable: |Bitte überprüfen Sie den in der json.Datei eingetragenen Servernamen
[Error] '{dfh}' is not a valid GUID value: |Bitte überprüfen Sie die eingetragenen GUID der eingetragenen DaVinci Serverdatei
[Error] Cannot open DaVinci file. No access rights.: |Bitte überprüfen Sie die Benutzerrechte, des in der json.Datei hinterlegten DaVinci Benutzers
[Error] Error sending data: (12029) Die Serververbindung konnte nicht hergestellt werden: |-
[Error] [Sdui] Keine Davinci Datei gefunden| -
[Error] [Sdui] Der hochgeladene Stundenplan stimmt mit dem aktuellen Plan nicht überein. Den Konflikt bitte unter "Perioden" im Admin Panel lösen.|Bitte wenden Sie sich direkt an SDUI
[ERROR] Error sending data: (12002) Das Zeitlimit für den Vorgang wurde erreicht | Bitte prüfen Sie in den Proxy-Einstellungen "Einstellungen automatisch erkennen"  ein Haken gesetzt ist und entfernen Sie diesen ggf.