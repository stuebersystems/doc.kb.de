# Ihre Magellan-Installation zieht auf einen neuen Serverrechner um?

Wir möchten Ihnen in diesem Artikel eine Übersicht bieten, an was alles zu denken ist beim Servertausch, damit die Weiterarbeit möglichst reibungslos erfolgen kann.


## Magellan und Firebird auf dem neuen Server installieren

Laden Sie die beiden Installationspakete herunter:

* [Firebird](https://download.stueber.de/bin/de/firebird/Firebird-2.5.8.27089_0_Win32.exe)
* [Magellan](https://download.stueber.de/bin/de/magellan/v7/magellan7.msi)

Eine Installationsanleitung finden Sie hier:

[Installationsanleitung Firebird](https://doc.magellan7.stueber.de/schulverwaltung/installation/Installation_Firebird/)
[Installationsanleitung Magellan](https://doc.magellan7.stueber.de/schulverwaltung/installation/server.installlieren/)

## Wichtige Dateien, die übernommen werden sollten

### Magellan7.FDB

Das ist die Datenbank, in der Ihre gesamten Schulverwaltungsdaten gespeichert sind. Diese Datei finden Sie bei Standardinstallation je nach Betriebssystem unter:


| Betriebssystem     | Speicherpfad                             |
|--------------------|------------------------------------------|
| Vista              | C:\Users\Public\Documents\Magellan 7\Datenbank\Magellan7.FDB |
| XP                 | C:\Dokumente und Einstellungen\All Users\Anwendungsdaten\Stueber Systems\Datenbank\Magellan7.FDB |
| Win2000            | C:\Dokumente und Einstellungen\All Users\Dokumente\Stueber Systems\Datenbank\Magellan7.FDB |
| Win7               | C:\Users\Public\Documents\Stueber Systems\Magellan 7\Datenbank\Magellan7.FDB |
| Windows Server2000 | C:\ProgramData\Documents\Stueber Systems\Magellan 7\Datenbank\Magellan7.FDB |
| Win10              | C:\Users\Public\Documents\Stueber Systems\Magellan 7\Datenbank\Magellan7.FDB |


> #### warning::Wichtig!
>
> Sollten Sie sich nicht sicher sein, wo genau sich diese Datenbank befindet, können Sie den genauen Pfad auch im Magellan 7 Administratormodul nachsehen. Sie finden den genauen Ablageort unter: `Datenbankverbindungen > Doppelklick auf die Verbindung> Unterpunkt Datenbank`.


### security2.FDB

Bitte sichern Sie vom alten Server die security2.FDB. 

Sie finden diese unter hier:

Betriebssystem|Speicherpfad
---|---
32Bit|  C:\Programme\Firebird\Firebird_2_5 
64Bit|C:\Program Files (x86)\Firebird\Firebird_2_5
  
Diese Datenbank enthält die Passwort- und Rechteinformationen (Passworte verschlüsselt). Daher muss auch bei einer Datenstrukturanpassung immer die Aktion "Synchronisiere Zugriffsrechte"  im Magellan Administrator ausgeführt werden.

Bei dieser Aktion werden die beiden Datenbanken, also die security2.FDB (Passwortdatenbank) und die magellan6.FDB (Schulverwaltungsdatenbank) miteinander abgeglichen, damit auch für die neu angefügten Teile der Datenbank der Zugriff für die Benutzer geklärt ist.

Beim Installieren von Firebird auf dem neuen Server wird an der selben Stelle wieder eine security2.FDB angelegt. Sie ersetzen diese durch die gesicherte und führen dann anschließend das "Synchronisieren der Zugriffsrechte aus". Sie finden diesen Punkt unter `Magellan Administrator > Datenbankpflege > Datenbank überprüfen > Zugriffsrechte synchronisieren`.

> #### primary::Hinweis
>
> Sichern Sie diese Datenbank nicht, kann sich kein Nutzer unter seinen gewohnten Zugangsdaten an der Magellan-Datenbank auf Ihrem neuen Server anmelden!

### Datenordner

Die folgenden Verzeichnisse enthalten von uns gelieferte Dateien, aber auch selbst erstellte oder angepasste Dateien.

Datenordner (Vorlagen, Skripte, Importe, Dokumente, Berichte, Datenordner):

| Betriebssystem      | Speicherpfad                             |
|---------------------|------------------------------------------|
| Vista               | C:\Users\Public\Documents\Magellan 7     |
| XP                  | C:\Dokumente und Einstellungen\All Users\Anwendungsdaten\Stueber Systems\Magellan 7 |
| Windows 2000        | C:\Dokumente und Einstellungen\All Users\Dokumente\Stueber Systems\Magellan 7 |
| Windows 7           | C:\Users\Public\Documents\Stueber Systems\Magellan 7 |
| Windows Server 2008 | C:\ProgramData\Documents\Stueber Systems\Magellan 7\ |


| Verzeichnis | Inhalt                                   |
|-------------|------------------------------------------|
| Vorlagen    | enthält die eigenen und gelieferten Serienbriefvorlagen |
| Berichte    | enthält alle Berichtsdateien, auch eigene oder selbst angepasste Berichte |
| Skripte     | enthält alle Skripte für Abiturberechnung. Statistik, Fortschreiben, Versetzen.... |
| Importe     | enthält die Schlüsseldateien zum Einlesen |
| Dokumente   | enthält die pro Schüler, Lehrer usw. gespeicherten Briefe, Dokumente u.ä. |
| Datenbank   | enthält Ihre Schulverwaltungsdatenbank und das Datawarehouse |

### Sonstige Dateien

| Datei        | Bedeutung                                |
|--------------|------------------------------------------|
| magellan.evm | Bitte nur übernehmen, wenn sich an den Ablagepfade auf dem neuen Server im Gegensatz zum bisherigen nichts ändert. Diese Datei speichert die eingestellten Pfade zu den Datenordnern und zu den Datenbanken Magellan6.FDB und Magellan6DWH.FDB. |
| magellan.lic | Diese Datei speichert die Lizenzierung.  |
| magellan.opt | Speichert die Einstellungen unter `Magellan > Extras > Optionen` |

Alle zu finden unter:

| Betriebssystem      | Speicherpfad                             |
|---------------------|------------------------------------------|
| Vista               | C:\ProgramData\Stueber Systems\Magellan 7 |
| XP                  | C:\Dokumente und Einstellungen\All Users\Anwendungsdaten\Stueber Systems\Magellan 7 |
| Windows 2000        | C:\Dokumente und Einstellungen\All Users\Anwendungsdaten\Stueber Systems\Magellan 7 |
| Windows 7           | C:\ProgramData\Stueber Systems\Magellan 7 |
| Windows Server 2008 | C:\ProgramData\Stueber Systems\Magellan 7\ |
| Win10               | C:\ProgramData\Stueber Systems\Magellan 7 |

### Anpassung für den ersten Clientrechner

Mit dem neuen Server müssten sich auch die Zugriffsinformationen von den Clients auf den Server ändern. Öffnen Sie nach erfolgter Übernahme von einem Client aus den Magellan-Administrator ohne Anmeldung.

![Wählen Sie im Feld `Datenbank`den Wert `Keine Anmeldung`.](/assets/images/admin.ohne.anmeldung.png)

Wechseln auf `Server-Verwaltung > Verbindungen verwalten > Starten > markieren Ihre Verbindung` und passen auf den Karten `Datenbank` und `Datenordner` die Pfadinformationen an.

> #### warning::Wichtig!
>
> Bitte denken Sie daran, das der Pfad aus Sicht des Servers erwartet wird, also bitte dort keinen Netzwerkpfad eingeben.

Wenn die Verbindung des ersten Arbeitsplatzrechners fertig angepasst ist, rufen Sie bitte Magellan auf und prüfen, ob Sie die Druckvorschau für einen Bericht sehen können. Weisen Sie zum Test einem Schüler etwas per Sammelzuweisung zu, im Anschluss löschen Sie den Eintrag wieder. Diese beiden Aktionen sollen letztlich nur bestätigen, ob die Pfadangaben korrekt waren. 

### Anpassung für den ersten Clientrechner

Diese Einstellungen müssten jetzt auf jedem weiteren Magellan-Client vorgenommen werden. Das können Sie genau wie im vorherigen Abschnitt vornehmen, oder Sie legen die Dateien, in denen diese Informationen gespeichert werden an zentraler Stelle ab und leiten Magellan beim Programmstart per `Magellan.paths`auf diese Dateien um.

Eine Anleitung dafür finden Sie im Abschnitt [Die Pathsdatei](https://doc.magellan7.stueber.de/installation/die-pathsdatei.html).

![Sichern Sie diese drei Dateien](/assets/images/pathsdateien.png)
