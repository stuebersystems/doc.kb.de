# Ihre Magellan-Installation zieht auf einen neuen Serverrechner um?

Wir möchten Ihnen in diesem Artikel eine Übersicht bieten, an was alles zu denken ist beim Servertausch, damit die Weiterarbeit möglichst reibungslos erfolgen kann.

`Stand Mai 2023`

## Magellan und Firebird auf dem neuen Server installieren

Laden Sie die beiden Installationspakete herunter:

* [Firebird](https://download.stueber.de/bin/de/firebird/Firebird-4.0.2.2816-0-Win32.exe)
* [Magellan für Windows 32-bit](https://download.stueber.de/bin/de/magellan/v10/magellan10_32.msi)
* [Magellan für Windows 64-bit](https://download.stueber.de/bin/de/magellan/v10/magellan10.msi)

Eine Installationsanleitung finden Sie hier:

[Installationsanleitung Firebird](https://doc.magellan.stueber.de/schulverwaltung/installation/version10/server.installieren/#installation-von-firebird-402)
[Installationsanleitung Magellan](https://doc.magellan.stueber.de/schulverwaltung/installation/version10/server.installieren/)

## Wichtige Dateien, die übernommen werden sollten

### Magellan10.fdb

Das ist die Datenbank, in der Ihre gesamten Schulverwaltungsdaten gespeichert sind. Diese Datei finden Sie bei Standardinstallation je nach Betriebssystem unter:


| Betriebssystem     | Speicherpfad                             |
|--------------------|------------------------------------------|
| Win7               | C:\Users\Public\Documents\Stueber Systems\Magellan 10\Datenbank\Magellan10.fdb |
| Windows Server2000 | C:\ProgramData\Documents\Stueber Systems\Magellan 10\Datenbank\Magellan10.fdb |
| Win10              | C:\Users\Public\Documents\Stueber Systems\Magellan 10\Datenbank\Magellan10.fdb |


**Sollten Sie sich nicht sicher sein, wo genau sich diese Datenbank befindet, können Sie den genauen Pfad auch im Magellan 9 Administratormodul nachsehen. Sie finden den genauen Ablageort unter: `Datenbankverbindungen > Doppelklick auf die Verbindung> Unterpunkt Datenbank`.**


### security10.fdb

Bitte sichern Sie vom alten Server die security4.fdb. 

Sie finden diese unter hier:

Betriebssystem|Speicherpfad
---|---
32Bit|  C:\Programme\Firebird\Firebird_4_0 
64Bit|C:\Program Files (x86)\Firebird\Firebird_4_0
  
Diese Datenbank enthält die Passwort- und Rechteinformationen (Passworte verschlüsselt). Daher muss auch bei einer Datenstrukturanpassung immer die Aktion "Synchronisiere Zugriffsrechte"  im Magellan Administrator ausgeführt werden.

Bei dieser Aktion werden die beiden Datenbanken, also die security4.fdb (Passwortdatenbank) und die magellan10.fdb (Schulverwaltungsdatenbank) miteinander abgeglichen, damit auch für die neu angefügten Teile der Datenbank der Zugriff für die Benutzer geklärt ist.

Beim Installieren von Firebird auf dem neuen Server wird an der selben Stelle wieder eine security4.fdb angelegt. Sie ersetzen diese durch die gesicherte und führen dann anschließend das "Synchronisieren der Zugriffsrechte aus". Sie finden diesen Punkt unter `Magellan Administrator > Benutzerverwaltung > Start > Zugriffsrechte synchronisieren`.

**Sichern Sie diese Datenbank nicht, kann sich kein Nutzer unter seinen gewohnten Zugangsdaten an der Magellan-Datenbank auf Ihrem neuen Server anmelden!**

### Datenordner

Die folgenden Verzeichnisse enthalten von uns gelieferte Dateien, aber auch selbst erstellte oder angepasste Dateien.

Datenordner (Vorlagen, Skripte, Importe, Dokumente, Berichte, Datenordner):

| Betriebssystem      | Speicherpfad                             |
|---------------------|------------------------------------------|
| Windows 7           | C:\Users\Public\Documents\Stueber Systems\Magellan 10 |
| Windows Server 2008 | C:\ProgramData\Documents\Stueber Systems\Magellan 10\ |


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
| magellan.evm | Bitte nur übernehmen, wenn sich an den Ablagepfade auf dem neuen Server im Gegensatz zum bisherigen nichts ändert. Diese Datei speichert die eingestellten Pfade zu den Datenordnern und zu den Datenbanken Magellan10.fdb  |
| magellan.lic | Diese Datei speichert die Lizenzierung.  |
| magellan.opt | Speichert die Einstellungen unter `Magellan > Extras > Optionen` |

Alle zu finden unter:

| Betriebssystem      | Speicherpfad                             |
|---------------------|------------------------------------------|
| Windows 7           | C:\ProgramData\Stueber Systems\Magellan 10 |
| Windows Server 2008 | C:\ProgramData\Stueber Systems\Magellan 10\ |
| Win10               | C:\ProgramData\Stueber Systems\Magellan 109 |

### Anpassung für den ersten Clientrechner

Mit dem neuen Server müssten sich auch die Zugriffsinformationen von den Clients auf den Server ändern. Öffnen Sie nach erfolgter Übernahme von einem Client aus den Magellan-Administrator ohne Anmeldung.

![Wählen Sie im Feld `Datenbank`den Wert `Keine Anmeldung`.](/assets/images/admin.ohne.anmeldung.png)

Wechseln auf `Server-Verwaltung > Verbindungen verwalten > Starten > markieren Ihre Verbindung` und passen auf den Karten `Datenbank` und `Datenordner` die Pfadinformationen an.

**Bitte denken Sie daran, das der Pfad aus Sicht des Servers erwartet wird, also bitte dort keinen Netzwerkpfad eingeben.**

Wenn die Verbindung des ersten Arbeitsplatzrechners fertig angepasst ist, rufen Sie bitte Magellan auf und prüfen, ob Sie die Druckvorschau für einen Bericht sehen können. Weisen Sie zum Test einem Schüler etwas per Sammelzuweisung zu, im Anschluss löschen Sie den Eintrag wieder. Diese beiden Aktionen sollen letztlich nur bestätigen, ob die Pfadangaben korrekt waren. 

### Anpassung für den ersten Clientrechner

Diese Einstellungen müssten jetzt auf jedem weiteren Magellan-Client vorgenommen werden. Das können Sie genau wie im vorherigen Abschnitt vornehmen, oder Sie legen die Dateien, in denen diese Informationen gespeichert werden an zentraler Stelle ab und leiten Magellan beim Programmstart per `Magellan.paths`auf diese Dateien um.

Eine Anleitung dafür finden Sie im Abschnitt [Die Pathsdatei](https://doc.magellan.stueber.de/schulverwaltung/installation/die-pathsdatei/).

![Sichern Sie diese drei Dateien](/assets/images/pathsdateien.png)
