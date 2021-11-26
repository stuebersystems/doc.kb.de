# Google-Token für den Kalenderübertrag zurücksetzen

In den Modulen DAVINCI und in DAVINCI LOOK gibt es die Möglichkeit Kalenderdaten in einen Google-Kalender zu übergeben.
Google liefert eine Software-basiertes Passwort-Token für die Authentifizierung.
Für weitere Abgleiche zwischen dem DAVINCI Kalender und Ihrem Google-Kalender wird diese Information gespeichert. 
Möchte man künftig mit einem anderen Google-Kalender abgleichen, muss der Google-Token wieder zurückgesetzt, also gelöscht werden.
Diese Daten werden in der Registry Ihres Rechners gespeichert unter:

```
HKEY_CURRENT_USER\Software\Stueber Systems\daVinci 6\Main\Google
```

