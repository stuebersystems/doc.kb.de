# Mapi-Schnittstelle: Welcher Client wird aufgerufen

Unsere Mailschnittstellen aus MAGELLAN oder DAVINCI rufen den Standard-Mailclient auf. 
Sollte nicht das Programm aufgerufen werden, dass Sie erwarten, kann es an folgendem Punkt liegen:

Es gibt die Möglichkeit einen Standard-Mailclient allgemein anzulegen (Einstellungen > Standard-Apps) und es kann einen nutzerbezogenen Eintrag geben, der beispielsweise nach der Installation des Mailclients (Soll xy Ihre Standard-Mailclient sein?) gesetzt wird.

Woher|Stelle in der Registrierungsdatenbank
--|--
aus den Standard-Apps| Computer\ **HKEY_LOCAL_MACHINE** \SOFTWARE\Clients\Mail
benutzerbezogen|Computer\ **HKEY_CURRENT_USER** \SOFTWARE\Clients\Mail

Dem nutzerbezogene Standard-Mailclient wird beim Aufruf der Funktionen mehr Gewicht beigemessen, damit könnten Sie beispielsweise unter `Start > Einstellungen (Zahnrad) > Standard-Apps > E-Mail`  "Outlook" wählen und dennoch würde beim Nutzen der Funktion immer beispielsweise "Mozilla Thunderbird" aufgerufen werden.

Was können Sie tun? Tragen Sie als Schlüsselwert den gewünschten Mailclient unter ` Computer\ **HKEY_CURRENT_USER** \SOFTWARE\Clients\Mail` ein.

1. Öffnen Sie die Registrierungsdatenbank (`Start > "regedit" eintippen > Enter`)
2. Gehe zu ` Computer\ **HKEY_CURRENT_USER** \SOFTWARE\Clients\Mail`
3. Doppelklicken Sie auf der rechten Seite auf den Schlüssel "Standard".
4. Tragen Sie den gewünschten Wert ("Mozilla Thunderbird" oder "Microsoft Outlook ") ein oder löschen den enthaltenen Wert, um den Eintrag aus den Standard-Apps zu nutzen.


