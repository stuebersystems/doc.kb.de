#	Die Paths-Datei

Die Optionsdateien werden für jeden Benutzer eines Computers angelegt. Wenn Sie im Netzwerk mit verschiedenen Clients arbeiten, können Sie eine PATHS-Datei verwenden, um globale Konfigurationen für alle Benutzer herzustellen: Dazu können Sie die XML-Textdatei daVinci.paths für daVinci bzw. die Datei daVinciLook.paths für daVinci LOOK verwenden. 

In diesen Dateien werden die Pfade für bestimmte Optionsdateien festgelegt. daVinci verwendet dann diese Pfadangaben, anstatt der Standardpfade. 

## Beispiel für eine PATH-Datei

```
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<Preferences>
 <Paths>
  <Entry Name="daVinciPrintFormatFile" Value="\\Mein_Server\...\Pathsdateien\daVinci.pfm"/>
  <Entry Name="daVinciOptionFile" Value="\\Mein_Server\...\Pathsdateien\daVinci.opt"/>
  <Entry Name="daVinciHTMLFormatFile" Value="\\Mein_Server\...\Pathsdateien\daVinci.hfm"/>
  <Entry Name="daVinciConfigurationFile" Value="\\Mein_Server\...\Pathsdateien\daVinci.cfg"/>
  <Entry Name="daVinciSiteFile" Value="\\Mein_Server\...\Pathsdateien\daVinci.site"/>
  <Entry Name="daVinciServerListFile" Value="\\Mein_Server\...\Pathsdateien\daVinci.servers"/>
  </Paths>
</Preferences>
```

> Bitte beachten Sie, dass anders als bei MAGELLAN, der Verweispfad jeweils mit dem Dateinamen enden muss.


Unter der Angabe „daVinciPrintFormatFile“ finden Sie diesen Pfad auch im Fenster `Extras > System-Informationen` wieder. Sie können die PATHS-Datei im Programmordner oder in den Datenordnern ablegen, siehe dazu die folgende Tabelle. Diese Ordner können je nach Betriebssystemversion variieren. Um welche Ordner es sich genau handelt, können Sie in daVinci bzw. in daVinci LOOK dem Fenster `Hilfe > System-Informationen` entnehmen.

Mögliche Ordner für die Datei “daVinci.paths“ |Mögliche Ordner für die Datei “daVinciLook.paths“ 
---|---
daVinciBinFolder	|daVinciLookBinFolder
daVinciDataFolder	|daVinciLookDataFolder
daVinciCommonDataFolder	|daVinciLookCommonDataFolder


> Die vollständige Pfadangabe zur aktuell verwendeten PATHS-Datei können Sie dem Eintrag „daVinciCustomPathsFile“ im Fenster `Hilfe > System-Informationen` entnehmen.

Die PATH-Datei kann die Pfadangaben für folgende Dateien festlegen:

**daVinci.paths**

Name|Datei|Beschreibung
---|---|---
daVinciOptionFile|daVinci.opt|Optionsdatei
daVinciHTMLFormatFile|daVinci.hfm|HTML Exportformate
daVinciPrintFormatFile|daVinci.pfm|Druckformate
daVinciConfigurationFile|daVinci.cfg|Aktuelle Login-Daten
daVinciSiteFile	|daVinci.site|Standortdaten (Schulname, Adresse, etc.)
daVinciServerListFile|daVinci.servers|Serververbindung und Startdatei

**daVinciLook.paths**

Name	|Datei	|Beschreibung
---|---|---
daVinciOptionFile|	daVinciLook.opt |	Optionsdatei
daVinciPrintFormatFile	|daVinci.pfm |	Druckformate
daVinciConfigurationFile	|daVinciLook.cfg|	Aktuelle Login-Daten
daVinciServerListFile|	daVinci.servers|	Serververbindung und Startdatei

