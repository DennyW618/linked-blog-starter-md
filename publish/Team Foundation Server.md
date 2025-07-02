

### 🔹TFS Einrichten

Eine Anleitung zum Einrichten des Team Foundation Servers findest du unter folgendem Link:

[Wie richte ich mir mit Visual Studio die TFS Verbindung ein? - Stack Overflow for Teams - eEvolution](https://stackoverflowteams.com/c/eevolution/questions/230)

### 🔹Checkin

**Was ist ein Checkin?**

Ein **Check-in** ist wie das Speichern und Teilen von Änderungen an einem gemeinsamen Projekt. Wenn jemand etwas bearbeitet hat, sorgt der Check-in dafür, dass alle anderen im Team die neuesten Änderungen sehen und nutzen können.

**Wie checke ich ein?**

1. Team Explorer -> Ausstehende Änderungen
2. Eingeschlossene Änderungen überprüfen (Nur das auswählen was man einchecken möchte)
3. Wahlweise den Checkin-Generator nutzen (unter Extras/Tools auswählen)
![[Pasted image 20250630150414.png]]
4. Unter *Developer* den eigenen Namen auswählen
5. Unter *Titel* das zugewiesene Work-Item auswählen 
6. **TaskId** wird automatisch eingefügt
7. Aktion wählen
8. Auf *Lade Kommentar* Klicken
9. **Ziel** manuell ersetzen (Zielprojekt) und **Beschreibung** Manuell ersetzen (Was wurde gemacht?)
10. Erstellten Text Kopieren (Manuell oder durch den **Kopieren** Button)
11. Text im Teamexplorer unter **Kommentar** einfügen
12. Mit **Task ID** verknüpfen
13. Auf **Einchecken** klicken

den Checkin-Generator findest du hier: [[Tools#🔹Checkin-Generator installieren]]

#### 🔹**Richtlinien für Checkin Kommentare**

[https://stackoverflowteams.com/c/eevolution/questions/29](https://stackoverflowteams.com/c/eevolution/questions/29 "https://stackoverflowteams.com/c/eevolution/questions/29")



### 🔹Mergen

Nachdem eine Aufgabe in eEvolution gelöst und eingecheckt und von des QS geprüft wurde (falls notwendig), muss die veränderte Version in die Version 11 überführt werden. Dafür ist ein Merge notwendig.

##### Mergen - in eEvolution 11.0:

1. eEvolution 11 vom tfs ziehen. eEvolution 6\Release\eEvolution 11.0.
2. Im Quellcodeverwaltungsexplorer Rechtsklick auf MainDev -> Branchen und Mergen -> Mergen...
3. "Ausgewählte Changesets" auswählen und bei ComboBox "Zielbranch" Evo 11 auswählen -> auf "Weiter" clicken.
4. Merge Changeset auswählen. -> "Fertig stellen".
5. Team Explorer -> ausstehende Änderungen -> Checkin nach Merge Richtlinien.
6. in eEvolution 11.0 navigieren (C:\dev\eEvolution 6\Release\eEvolution 11.0).
7. CMD öffnen -> BuildDebug.bat ausführen.
8. Bei mehreren Checkins muss die neuste Version von eEvolution 11 abgerufen werden um Versionskonflikte zu vermeiden.


[[Startseite]]
