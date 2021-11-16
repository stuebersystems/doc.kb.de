# Einführung

MAGELLAN und DAVINCI ist Schulorganisationssoftware für alle deutschen Bundesländer und alle Schularten. Entsprechend der Kulturhoheit der Bundesländer müssen die Programme unterschiedliche landesspezifische Zeugnisformulare, Verordnungen und Landesstatistiken unterstützen. Innerhalb des jeweiligen Landes muss dabei oft nochmals nach Schularten differenziert werden. Betrachtet man die Unterschiede der Formulare, Verordnungen und Landesstatistiken, stellt man fest, dass sich alle irgendwie ähneln.

Die überwiegenden Gemeinsamkeiten sind der Grund dafür, dass wir alle Informationen zur Landesanpassung in den Programmen MAGELLAN und DAVINCI in einem einzigen Dokument zusammengefasst haben. So können Sie z.B. aus der Beschreibung eines Zeugnisformulars für ein ganz anderes Bundesland zum Schluss kommen, dass Sie dieses Formular mit geringem Aufwand an die Bedürfnisse Ihres Bundeslandes anpassen könnten.

!!! info "Hinweis"

     Diese Dokumentation versteht sich als Ergänzung der landesspezifischen Besonderheiten zu den Standarddokumentationen für [**MAGELLAN**](https://doc.magellan7.stueber.de/) und [**DAVINCI**](https://doc.davinci6.stueber.de/).

Diese Dokumentation teilt sich in zwei Bereiche:

Bereiche|Informationen
--|--
[Skripte](https://doc.la.stueber.de/skriptueberblick/)|Dieser Bereich teilt sich in die Unterbereiche
[Berichte](https://doc.la.stueber.de/berichte/01_uebersicht/)| Dieser Bereich listet für die Berichte (Zeugnisse, Listen usw) der Auslieferung die notwendigen Eingaben auf.

## Allgemeines

Allgemeine Formulare, die Zeugnisformulare und deren Anwendung werden im Modul `MAGELLAN-Berichte` beschrieben, das Sie nach der Installation unter `Start > Programme > STÜBER SYSTEMS` finden.

### DAVINCI Landesanpassungen

Als Teil der DAVINCI Landesanpassung werden folgende landesspezifische Funktionen bzw. Daten zur Verfügung gestellt bzw. installiert:

1. Die Fachwahlüberprüfung für Ihr Bundesland Sie kann Teil von DAVINCI KURSPLAN sein.

2. Die Lehrer-Soll-Berechnungsschlüssel, d.h. die Mehrarbeits- und Ermäßigungsgründe für die Lehrer. Sie werden als txt-Datei für Ihr Bundesland installiert.

### MAGELLAN Landesanpassungen

Als Teil der Landesanpassung werden in MAGELLAN folgende landesspezifische Funktionen bzw. Daten zur Verfügung gestellt bzw. installiert:

* Die Fachwahlüberprüfung unter `MAGELLAN > Abitur > Fachwahl` für Ihr Bundesland
* Die Schlüsselverzeichnisse für Ihr Bundesland
* Die Abiturqualifikationsberechnungen für Ihr Bundesland
* Die Landesstatistik ([siehe gesonderte Dokumentation](https://doc.ls.stueber.de/))

## Schlüsselverzeichnisse

Schlüsselverzeichnisse spielen in MAGELLAN und DAVINCI eine zentrale Rolle.
Jeder Eintrag in diesen Verzeichnissen besteht mindestens aus `Kürzel` und `Schlüssel`.
Das `Kürzel` wird in MAGELLAN und DAVINCI zur Anzeige verwendet, der `Schlüssel` wird für Berichte, die Landesstatistik und für die Fachwahlüberprüfung bzw. die Abiturqualifikation verwendet.

!!! info "Hinweis"

    Viele Werte sind durch den Import der Schlüsselverzeichnisse bereits korrekt gefüllt, bitte prüfen Sie aber dennoch vorab, ob die pro Skript oder Bericht erwarteten Werte in Ihrem Verzeichnis enthalten sind oder ggf. ergänzt werden müssen. Welche genau das sind, beschreiben wir im jeweiligen Unterpunkt pro Skript oder für Berichte im Modul MAGELLAN BERICHTE.

Beim Datenabgleich zwischen MAGELLAN und DAVINCI werden die Schlüsselverzeichnisse `Unterrichtsarten` und `Fachstatus` aus Sicherheitsgründen nicht mit abgeglichen.

### Lehrer-Soll-Berechnungsschlüssel

Die Lehrer-Soll-Berechnungsschlüssel werden in DAVINCI für das individuelle Soll-Berechnungsschema des einzelnen Lehrers benötigt. Mit ihnen geben Sie an, welche Ermäßigungs- und Mehrarbeitsstunden jeder Lehrer erhält. Die Lehrer-Soll-Berechnungsschlüssel geben Sie im DAVINCI-Basismodul im Stammdatenfenster auf der Registerkarte `Lehrer`  über `Arbeitszeitkonto bearbeiten` (rechte Maustaste auf Lehrerkürzel) ein.
Bei der Installation von DAVINCI werden alle verfügbaren Soll-Berechnungsschlüssel im Unterverzeichnis „Schlüssel“ im DAVINCI-Verzeichnis installiert. Die Schlüsseldateien sind nach dem jeweiligen Bundesland benannt und haben die Endung „.key“.

### Allgemeine Abkürzungen

Folgende Abkürzungen werden in den nachfolgenden Kapiteln verwendet:

| Abkürzung   | Bezeichnung                  |
|-------------|------------------------------|
| ABS         | allgemeinbildende Schule     |
| ABI         | Abitur                       |
| AG          | Abendgymnasium               |
| APO         | Abiturprüfungsordnung        |
| AS          | Abschlusszeugnis             |
| AZ          | Abgangszeugnis               |
| BBS         | berufsbildende Schule        |
| BF          | Berufsfachschule             |
| BGJ         | Berufsgrundschuljahr         |
| BG          | Berufliches Gymnasium        |
| BKO         | Berufskolleg                 |
| BS          | Berufsschule                 |
| BV          | Berufsvorbereitende Maßnahme |
| BVJ         | Berufsvorbereitungsjahr      |
| FG          | Fachgymnasium                |
| FO oder FOS | Fachoberschule               |
| FSP         | Fremdsprache                 |
| FS          | Fachschule                   |
| GES         | Gesamtschule                 |
| GS          | Grundschule                  |
| GY          | Gymnasium                    |
| HA          | Handelsschule                |
| HBF         | Höhere Berufsfachschule      |
| HHA         | Höhere Handelsschule         |
| HJ          | Halbjahr                     |
| HJZ         | Halbjahreszeugnis            |
| HS          | Hauptschule                  |
| IGS         | Integrierte Gesamtschule     |
| JZ          | Jahreszeugnis                |
| KO          | Kolleg                       |
| MIT         | Mittelschule                 |
| REG         | Regionale Schule             |
| RGL         | Regelschule                  |
| RS          | Realschule                   |
| SEK         | Sekundarschule               |
| SO          | Sonderschule                 |
| ÜZ          | Übergangszeugnis             |
| WG          | Wirtschaftsgymnasium         |

### Abkürzungen in Meldungen

Als Ergebnis der Fachwahlüberprüfung in MAGELLAN und DAVINCI-Kursplan werden ggf. Hinweise ausgegeben, z.B. „NW, FS nicht abgedeckt“.

Die Bedeutung der Abkürzungen können Sie der nachfolgenden Tabelle entnehmen:

| Merkmal | Bedeutung                                |
|---------|------------------------------------------|
| D       | Deutsch                                  |
| FS      | Fremdsprachen                            |
| Ge      | Geschichte                               |
| Che     | Chemie                                   |
| M       | Mathematik                               |
| NW      | Naturwissenschaft                        |
| Sport   | Sport                                    |
| R/Eth   | Religion/Ethik                           |
| Phy     | Physik                                   |
| Bio     | Biologie                                 |
| Inf     | Informatik                               |
| GK      | Gemeinschaftskunde bzw. Gesellschaftskunde |
| Ku      | Kunst                                    |
| KF      | Künstlerisches Fach, d.h. Kunst bzw. Musik |
| Pol     | Politische Bildung bzw. Politik          |
| Spiel   | Darstellendes Spiel                      |
| LF      | Leistungsfach                            |
| Phi     | Philosophie                              |
| Bereich | Aufgabenbereich bzw. Aufgabenfeld        |
| Erd     | Erdkunde                                 |

### Abkürzungen der Bundesländer

Folgende Abkürzungen werden für die Bundesländer verwendet:

| Abkürzung | Bezeichnung                          |
|-----------|--------------------------------------|
| ALL       | Allgemein, d.h. bundeslandunabhängig |
| BAW       | Baden-Württemberg                    |
| BAY       | Bayern                               |
| BRA       | Brandenburg                          |
| BRE       | Bremen                               |
| HAM       | Hamburg                              |
| HES       | Hessen                               |
| MVP       | Mecklenburg-Vorpommern               |
| NIE       | Niedersachsen                        |
| NRW       | Nordrhein-Westfalen                  |
| RLP       | Rheinland-Pfalz                      |
| SAA       | Sachsen-Anhalt                       |
| SAR       | Saarland                             |
| SAC       | Sachsen                              |
| SHL       | Schleswig-Holstein                   |
| THÜ       | Thüringen                            |

## Berichte

Berichte definieren in MAGELLAN das Layout und den Inhalt von Zeugnissen, Übersichten, Listen usw. Berichte sind als Dateien im MAGELLAN-Verzeichnis Berichte abgelegt.  Diese Dateien bzw. Berichte wurden mit dem Berichtsgenerator „Crystal Reports“ erstellt und können mit ihm auch wieder verändert werden.

### Informationen zu Berichten

!!! info "Hinweis"

     Weitere Informationen zu Berichten veröffentlichen wir über das [Modul Berichte](https://doc.magellan7.stueber.de/schulverwaltung/howto/berichte-verz.html). Sie finden den Aufruf unter `Start > Programme > Stueber Systems > MAGELLAN 7 Berichte`. 

Sie haben in diesem Informationsmodul in der oberen Menüleiste die Möglichkeit nach der Region und der Art des Berichtes zu filtern. Per Doppelklick auf eine Berichtsbezeichnung werden Ihnen zusammengefasst die Anmerkungen (also, was genau ist wo im Programm zu erfassen) angezeigt. Die Anmerkungen können auch als Textdatei exportiert werden.

### Wenn Sie selbst Berichte erstellen möchten

Alle in diesem Dokument erwähnten Crystal-Reports-Berichte für Listen und Zeugnisse können mit dem kostenlos mitgelieferten Runtime-Modul von MAGELLAN ausgedruckt werden. Wenn Sie lediglich die mitgelieferten Zeugnisformulare verwenden, ohne Änderungen am Layout vorzunehmen, benötigen Sie keinen Druckreportgenerator, da bereits eine Runtime-Version des in MAGELLAN verwendeten Crystal Reports-Berichtsgenerators mitinstalliert wird. Wenn Sie Berichte selbst verändern oder erstellen möchten, benötigen Sie eine Lizenz von Crystal Reports.

!!! info "Hinweis"

    STÜBER SYSTEMS bietet exklusiv für MAGELLAN eine spezielle Schulversion von Crystal Reports Professional an. Über Schulungstermine informieren wir [hier](http://www.stueber.de/training.php)

Wenn Sie neue Berichte erstellen bzw. vorhandene verändern möchten, benötigen Sie einen Berichtsgenerator, d.h. ein Programm, mit dem Sie Berichte erstellen und verändern können. MAGELLAN verwendet ausschließlich den Berichtsgenerator Crystal Reports. In MAGELLAN werden daher ausschließlich Crystal Reports Berichte mitgeliefert. Sie können eine spezielle Schulversion von Crystal Reports von STÜBER SYSTEMS beziehen.

Sie können Berichte alternativ auch in Access erstellen. Wie Sie Access an die MAGELLAN-Datenbank anbinden. Bitte beachten Sie, dass gerade schwierige Berichte wie Zeugnisberichte  in Crystal Reports wesentlich effizienter erstellt werden können.

!!! info "Hinweis"

    Falls Sie selbst in Crystal Reports Berichte erstellen möchten, finden Sie die dazu notwendigen Informationen in der [MAGELLAN 6 Datenstruktur](https://doc.magellan7-toolbox.stueber.de/datenstruktur/).

### Berichte im Auftrag erstellen lassen

Optional können Sie STÜBER SYSTEMS beauftragen, für Sie die benötigten Formulare bzw. Berichte zu erstellen. Sie erhalten dann von STÜBER SYSTEMS die entsprechenden Crystal Reports Berichtsdateien, die Sie lediglich in das entsprechende Berichtsverzeichnis kopieren müssen. Schicken Sie dazu Ihre entsprechenden Papiervorlagen und ein ausgefülltes Beispiel an STÜBER SYSTEMS. Sie erhalten dann ein Angebot über die Kosten für die Erstellung der Berichte.

### Layout der Berichte

Die im Lieferumfang von MAGELLAN standardmäßig enthaltenen Berichte entsprechen den offiziellen Vorschriften oder orientieren sich, soweit keine Vorschriften verfügbar waren, an den in der Praxis von Schulen verwendeten Vorlagen. Die Berichte verwenden in der Regel die Windows Standardschriftart Arial. Diese Schriftart ist auf jedem Windows-PC vorhanden. Sollten Sie in selbst erstellten Berichten andere Schriftart verwenden, müssen Sie darauf achten, dass die entsprechenden Schriftarten auch auf dem jeweiligen PC, von dem aus gedruckt wird, vorhanden sind.

### Berichtsdateinamen

Jeder ausgedruckte Bericht enthält klein gedruckt links unten den Namen des Berichts. So können Sie z.B. bei Supportanfragen den Bericht eindeutig identifizieren. Sie können den Namen ggf. über Crystal Reports aus dem Bericht löschen. Die Dateinamen entsprechen folgender Konvention, die wir anhand eines Beispiels  erläutern.

Der folgende Dateiname bezeichnet ein Halbjahreszeugnis für Gymnasien in Rheinland-Pfalz.

**Beispiel:** `RLP-GY-HJ (2spaltig mit FSP).rpt`

| RLP        | GY                  | HJ                                       | (2-spaltig mit FSP) | .rpt                            |
|------------|---------------------|------------------------------------------|---------------------|---------------------------------|
| Bundesland | Schulart, Schulform | Zeugnisart, wie Jahres- oder Halbjahreszeugnis oder Abschluss | Bemerkung           | Dateiendung von Crystal Reports |
