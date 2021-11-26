# Serienmails: Mapi-Fehler

[1]:/assets/images/Magellan/11.png
[2]:/assets/images/Magellan/12.png

Es liegt nicht an MAGELLAN direkt, sondern an einer falschen Konfiguration der MAPI-Schnittstelle von Microsoft:

 Lösung: Eine Nachkonfiguration in der Registry.

Erstens:

Beenden Sie Outlook und öffnen Sie den Registrierungs-Editor. Verwenden Sie hierzu je nach Ihrer Windows-Version eines der folgenden Verfahren.

* Windows 10, Windows 8.1 und Windows 8: Drücken Sie WINDOWS-TASTE+R, um das Dialogfeld „Ausführen“ zu öffnen. Geben Sie regedit.exe ein, und klicken Sie dann auf **OK**.
* Windows 7: Klicken Sie auf „Start“, geben Sie in das Suchfeld die Zeichenfolge  **regedit.exe** ein, und drücken Sie dann die **EINGABETASTE**.

Zweitens:

Suchen Sie den folgenden Schlüssel in der Registrierung und wählen Sie ihn aus: `HKEY_LOCAL_MACHINE\SOFTWARE\Wow6432Node\Microsoft\Windows Messaging Subsystem\MAPI`

Unter Windows 64-bit muss man den Schlüssel neu anlegen und/oder den Wert anpassen.

* Gehen Sie über die rechte Maustaste im rechten Fenster auf "Neu", wählen Sie hier "Zeichenfolge" und benennen diese **MAPI**!

[![Beschriftung][1]][1]

* Anschließend gehen Sie über die rechte Maustaste auf diesen neuen Eintrag und wählen "Ändern", hier tragen Sie im Feld "Wert" eine **1** ein.

[![Beschriftung][2]][2]

* Schließen Sie den Registrierungs-Editor und starten Sie Outlook.
