# AV_KASO Abgleich
Verantwortlicher: Andrea Lüscher

## Beschreibung:
Die Katasterschätzung verwaltet die Grundstücke inkl. der Grundstücksflächen in einer DB (KASO von aXenta). Die Fläche ist einer der Faktoren, mit welchem der Katasterwert errechnet wird. Die Nachführung der Grundstücke erfolgt mittels analoger Anzeige vom Grundbuch.
Die Grundstücksfläche wird aus dem Grenzverlauf, der in der amtlichen Vermessung (AV) festgehalten ist, errechnet. Die Fläche wird von der amtlichen Vermessung an das Grundbuch übergeben und das Grundbuch teilt die Fläche mittels Anzeige der Katasterschätzung mit.
Die Grundstücksdaten der Katasterschätzung, des Grundbuchs und der amtlichen Vermessung sollten identisch sein. Aufgrund des Vergleichs vom August 2016 hat sich gezeigt, dass die Daten der Katasterschätzung und der amtlichen Vermessung nicht identisch sind.
Das Monitoring „Abgleich KASO-AV“ ist ein Arbeitstool für die Katasterschätzung, damit die Daten der KASO nachgeführt resp. bereinigt werden können.

## Import und Datenumbau:
Die Daten der Katasterschätzung werden von deren Oracle-DB kopiert und in unsere Pub-DB eingefügt. Anschliessen werden die Daten so umgebaut (verglichen), dass lediglich die Einträge in der Differenztablle aufgeführt werden, bei welchen die KASO-Daten nicht mit den AV-Daten übereinstimmen. Folgendes wird geprüft:

* Flächendifferenz zwischen AV und KASO
* unterschiedliche Grundstücksarten in AV und KASO
* Grundstück nur in der AV vorhanden
* Grundstück nur in KASO vorhanden

**Gretljob:** https://github.com/sogis/gretljobs/tree/master/agi_av_kaso_abgleich_pub

**Layer Web GIS Client:** "Differenzen AV-KASO" (geschützt)


## Betriebshandbuch:
Das Betriebshandbuch liegt unter: H:\BJSVW\Agi\GDI\Betrieb\AV_Kaso_Abgleich\Betriebshandbuch.doc
