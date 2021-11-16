# HTTPS Protokoll

Aktuell muss man bei der Umstellung der Webbseite von http auf https ein paar Template-Textdateien manuell editieren:

1. Bitte wechseln Sie in das Verzeichnis ``C:\ProgramData\Stueber Systems\daVinci 6\HTML\HTML``.

2. Öffnen Sie nacheinander alle HTML-Textdateien und ändern Sie alle Verweise von 
[http://www.stueber.de/assets/...](http://www.stueber.de/assets/...) auf [https://www.stueber.de/assets/...](https://www.stueber.de/assets/...).

    **Beispiel:**

    aus

    **&lt;link rel="stylesheet" href="**[**http://www.stueber.de/assets/davinci/css/bootstrap.min.css**](http://www.stueber.de/assets/davinci/css/bootstrap.min.css)**&gt;**

    wird

    **&lt;link rel="stylesheet" href="**[**https://www.stueber.de/assets/davinci/css/bootstrap.min.css**](https://www.stueber.de/assets/davinci/css/bootstrap.min.css)**&gt;**

!!! info "Hinweis"

    Am einfachsten geht dies mit einem Texteditor wie [Notepad++](https://notepad-plus-plus.org/), dort können Sie es mit einem einzigen Befehl für alle Dateien durchführen.

Nun Exportieren Sie bitte noch einmal nach HTML. Jetzt sollte ein Einsatz unter https keine Probleme mehr bereiten.
