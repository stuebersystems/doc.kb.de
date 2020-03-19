# Serienmails: Mapi-Fehler

Es liegt nicht an MAGELLAN direkt, sondern an einer falschen Konfiguration der MAPI-Schnittstelle von Microsoft:

 Lösung: Eine Nachkonfiguration in der Registry ist erforderlich

 1. Beenden Sie Outlook

 2. Öffnen Sie den Registrierungs-Editor. Verwenden Sie hierzu je nach Ihrer Windows-Version eines der folgenden Verfahren.

* Windows 10, Windows 8.1 und Windows 8
  : Drücken Sie WINDOWS-TASTE+R, um das Dialogfeld „Ausführen“ zu öffnen. Geben Sie regedit.exe
   ein, und klicken Sie dann auf   **OK**
  .
* Windows 7
  : Klicken Sie auf „Start“, geben Sie in das Suchfeld die Zeichenfolge  **regedit.exe** ein, und drücken Sie dann die  **EINGABETASTE**

 3. Suchen Sie den folgenden Schlüssel in der Registrierung, und wählen Sie ihn aus.

`HKEY_LOCAL_MACHINE\SOFTWARE\Wow6432Node\Microsoft\Windows Messaging Subsystem`

 4. Unter WIndows 64-bit muss man folgenden Einstellung vornehmen - Wenn der Schlüssel MAPI dort nicht existiert \(das müsste bei Ihnen der Fall sein\), müsen Sie diesen wie folgt manuell anlegen.

5. Gehen Sie über die rechte Maustaste im rechten Fenster auf "Neu", wählen Sie hier "Zeichenfolge" und benennen diese

**MAPI**![](/assets/sshot-1.png)

 6. Anschließend gehen Sie über die rechte Maustaste auf  diesen neuen Eintrag und wählen "Ändern", hier tragen Sie im Feld "Wert" eine **1** ein.

![](/assets/sshot-2.png)

 7. Schließen Sie den Registrierungs-Editor.

 8. Starten Sie Outlook.
