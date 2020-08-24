# afu_geotope

Verantwortlicher: Andrea Lüscher

## Beschreibung:
Infolge einer Ablösung des veralteten Servers «srsofaioi4531», mussten die Anwendungen INGESO, IS-Boden und VSB abgelöst werden. Siehe auch [Projektmanagementplan]("H:\BJSVW\Agi\Projekte\AFU\Ablösung INGESO VSB ISBoden Anwendungen\Projektmanagment\Projektmanagementplan_v01.docx").

## QGIS Projekte:
### Erfassung:
Zum Erfassen der Daten in der Edit-DB.

H:\BJSVW\Agi\Projekte\AFU\Ablösung INGESO VSB ISBoden Anwendungen\AP_Datenumbau_Realisiserung\Geotope_Erfassung_Produktionsumgebung.qgz

### Auswertung:
Zum Filtern von Attributwerten aus der Pub-DB.

H:\BJSVW\Agi\Projekte\AFU\Ablösung INGESO VSB ISBoden Anwendungen\AP_Datenumbau_Realisiserung\Geotope_Auswertung_Produktionsumgebung.qgz

## Datenumbau:
Die Daten werden mittels einem Gretljob von der Edit-DB in die Pub-DB geschrieben.

**Gretljob afu_geotope_pub:** https://github.com/sogis/gretljobs/tree/master/afu_geotope_pub

## DB Schema:
Edit-DB: afu_geotope

Pub-DB: afu_geotope_pub
