# afu geotope

Verantwortliche: Andrea Lüscher

## Beschreibung:
Infolge einer Ablösung des veralteten Servers «srsofaioi4531», mussten die Anwendungen INGESO, IS-Boden und VSB abgelöst werden. Siehe auch Projektmanagementplan: `H:\BJSVW\Agi\Projekte\AFU\Ablösung INGESO VSB ISBoden Anwendungen\Projektmanagment\Projektmanagementplan_v01.docx`.

Die Daten werden mittels einem QGIS Projekt in der Edit-DB erfasst und in einem QGIS-Projekt mit den Daten aus der Pub-DB ausgewertet. Im Web GIS Client werden die Daten aus der Pub-DB abgebildet. Bei einer Datenänderung, werden die aktuellen Daten  von den MA des AFU via eines Greljobs von der Edit-DB in die Pub-DB geschrieben.

Damit die Erfassung und Auswertung einfacher ist, gibt es für die Erfassung und die Auswertung ein eigenes QGIS-Projekt mit einem eigenen QGIS-Profile. In diesen Profiles sind nur die Werkzeuge aktiviert, welche wirklich benötigt werden.

Im Web GIS Client kann pro Geotop das Objektblatt "Inventar der geowissenschaftlich schützenswerten Objekte" geöffnet werden. Das Objektblatt wird mittels einem Jasper-Report erstellt.

## QGIS Projekte:
### Erfassung:
Zum Erfassen der Daten in der Edit-DB.

QGIS Projekt: `H:\BJSVW\Agi\Projekte\AFU\Ablösung INGESO VSB ISBoden Anwendungen\AP_Datenumbau_Realisiserung\Geotope\Geotope_Erfassung_Produktionsumgebung.qgz`

ini-File: `H:\BJSVW\Agi\Projekte\AFU\Ablösung INGESO VSB ISBoden Anwendungen\AP_Datenumbau_Realisiserung\Geotope\Geotop_Erfassung.ini`

### XXX

### Auswertung:
Zum Filtern von Attributwerten aus der Pub-DB.

QGIS-Projekt: `H:\BJSVW\Agi\Projekte\AFU\Ablösung INGESO VSB ISBoden Anwendungen\AP_Datenumbau_Realisiserung\Geotope\Geotope_Auswertung_Produktionsumgebung.qgz`

ini-File: `H:\BJSVW\Agi\Projekte\AFU\Ablösung INGESO VSB ISBoden Anwendungen\AP_Datenumbau_Realisiserung\Geotope\Geotop_Auswertung.ini`

## Datenumbau:
Die Daten werden mittels einem Gretljob von der Edit-DB in die Pub-DB geschrieben.

**Gretljob afu_geotope_pub:** https://github.com/sogis/gretljobs/tree/master/afu_geotope_pub

## DB Schema:
Edit-DB: `afu_geotope`

Pub-DB: `afu_geotope_pub`

## Web GIS Client:
Layergruppe: `ch.so.afu.geotope*`

Jasper-Report: Template im AGDI `afu_geotope`

## Anleitungen:
### Erfassung im QGIS: 
`H:\BJSVW\Agi\Projekte\AFU\Ablösung INGESO VSB ISBoden Anwendungen\AP_Datenumbau_Realisiserung\Geotope\Anleitung_Erfassung_Geotope.docx`

### Auswertung im QGIS: 
`H:\BJSVW\Agi\Projekte\AFU\Ablösung INGESO VSB ISBoden Anwendungen\AP_Datenumbau_Realisiserung\Geotope\Anleitung_Auswertung_Geotope.docx`

