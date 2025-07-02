

### 🔹 Allgemeine Coding Challenges

- [LeetCode](https://leetcode.com/): Eine beliebte Plattform zum Üben von Programmieraufgaben, besonders für technische Bewerbungsgespräche und algorithmisches Denken.

- [Coding Dojo Katas](https://codingdojo.org/kata/)Eine Sammlung von kleinen, wiederholbaren Programmierübungen („Katas“) zur Verbesserung von Codequalität und Problemlösungsfähigkeiten.

- [Clean Code Developer – Coding Dojo](https://ccd-school.de/coding-dojo/): Eine deutschsprachige Plattform mit Fokus auf sauberen Code und Softwarehandwerk, inklusive Dojos zum Üben guter Programmierpraktiken.
- 

### 🔹 Übungsprojekt (in mehrere Abschnitte aufgeteilt)


🟢**Stufe 1:** Grundlagen – Klassen und Objekte

**Ziel:** Einführung in Klassen, Attribute und Objektinstanzen.

-Erstelle eine Klasse Mitglied mit den Attributen:

**id** (zunächst manuell vergeben)

**name**

**alter**

**mitgliedsstatus**

- Erstelle 2–3 Objekte dieser Klasse im Code.

- Gib Name und Mitgliedsstatus dieser Mitglieder in der Konsole aus.

➡️ **Lernziel:** Klassen, Konstruktor, Attribute, Objektinstanzen, einfache Konsolenausgabe.


🟡 **Stufe 2:** Vergleich und Kategorisierung

**Ziel:** Einführung in Bedingungen, Listen und einfache Logik.

-Speichere alle Mitglieder in einer Liste.
-Prüfe, ob es doppelte Mitglieder gibt (gleicher Name, Alter, Status).
-Gib Mitglieder nach Alterskategorie aus:
-Kinder: unter 13
-Teenager: 13–19
-Erwachsene: 20+

➡️ **Lernziel:** Listen, Schleifen, Bedingungen, Vergleichslogik.


🟠 **Stufe 3:** Konsolenmenü und Benutzerinteraktion

Ziel: Einführung in Benutzereingaben und einfache Menüs.

Erstelle ein Menü mit:
-**[1]** Neues Mitglied hinzufügen
-**[2]** Alle Mitglieder anzeigen
-**[10]** Beenden

-Eingabe aller Attribute über Konsole (ID noch manuell).

➡️ **Lernziel:** input(), Schleifen, einfache Menüführung.


🔵 **Stufe 4:** Automatische ID-Vergabe und Validierung

Ziel: Einführung in Validierung und Fehlerbehandlung.

-**ID** wird automatisch vergeben (z. B. mit einem Zähler).
-Validierung:
    **Name:** nur Buchstaben, mindestens 3 Zeichen
    **Alter:** muss eine Zahl sein
    
-**Bonus:** Wiederhole Eingabe bei Fehlern.

➡️ **Lernziel:** Fehlerbehandlung (try/except), benutzerdefinierte Fehlermeldungen, Validierung.


🟣 **Stufe 5:** JSON-Speicherung

Ziel: Einführung in **Dateispeicherung** und **JSON.**

Menü erweitern:
-**[3]** Mitglieder als JSON speichern
-**[4]** Mitglieder aus JSON laden
-**Speicherort** z. B. mitglieder.json

➡️ **Lernziel:** Dateioperationen, JSON, Serialisierung/Deserialisierung.


🔴 **Stufe 6:** Zufällige Mitglieder generieren

Ziel: Einführung in zufällige Daten und Programmstart-Logik.

-Wenn keine JSON-Datei vorhanden oder leer:
-Erzeuge 3–5 zufällige Mitglieder beim Start.

➡️ **Lernziel:** os.path, Zufallsfunktionen, Startlogik.


🟤 **Erweiterung:** GUI mit WinForms und SQLite (optional, fortgeschritten)

Ziel: Einführung in GUI-Programmierung und Datenbanken.

-MVVM-Struktur
-SQLite statt JSON
-Mitglieder können bearbeitet und gelöscht werden

➡️ Lernziel: GUI-Design, Datenbankzugriff, MVVM-Architektur.



### 🔹 Konkretes Übungsprojekt (im ganzen)

#### - Eine Erste Übungsaufgabe -

**Ziel:** Es soll eine Verwaltungssoftware erstellt werden, die "Mitglieder" verwalten kann.
Bitte Klassen- und Ordnerstruktur so wählen, wie es für euch Sinn macht.

Mitglieder sollen diese Attribute haben.

- Id   
- Namen  
- Alter  
- Mitgliedstatus

**Beispiel:**  
Bob, 29, Kassenwart

##### 1.  Erstellt 2-3 Objekte dieser Datenklasse im Code, zum Testen der Implementierung.

Die Software soll folgende Funktionalitäten haben:

- Sie kann den Namen und Mitgliedsstatus von Mitgliedern ausgeben.  
- Sie kann überprüfen, ob es Mitglieder mit identischen Namen, Alter und Mitgliedsstatus gibt. Falls ja, soll sie die entsprechende id dieser ausgeben.  
- Es sollen alle Benutzer einer bestimmten Alterskategorie ausgeben werden. Hierbei sollen diese so (oder so ähnlich) kategorisiert und ausgegeben werden:

x Mitglieder sind Kinder (Alter unter 13)  
y Mitglieder sind Teenager (Alter zwischen 13-19).  
z Mitglieder sind Erwachsene (Alter 19+)
#####  2. Erstellt ein kleines Menü in der Konsole:

[1] Neuen Benutzer hinzufügen

[2] Alle Benutzer anzeigen

[10] Beenden

Dabei sollen alle Attribute von dem Benutzer eingegeben werden können.

##### 3. Id soll nicht mehr abgefragt werden und soll automatisch vergeben werden. Dafür darf jede Id nur einmal vergeben werden.

##### 4. Validierungs- und Exception Handling:  

**Eingaben sollen nur akzeptiert werden, wenn:**  

- der Namen länger als 2 Buchstaben ist  
- der Name nur Buchstaben enthält
- Alter soll eine benutzerdefinierte Fehlermeldung ausgeben, wenn keine gültige Zahl eingegeben wurde (anstatt einer Exception)  
- 
**Bonus:** Falls der Benutzer was falsches eingibt, soll das Programm solange danach fragen, bis es eine gültige Eingabe bekommt

##### 5. Es sollen diese Punkte in der Konsole eingefügt werden:  

[3] Mitglieder als JSON speichern

[4] Mitglieder aus JSON laden

Der Name und Speicherort der JSON ist frei von euch wählbar.

##### 6. Zufällige Mitglieder generieren:

Sollte keine JSON existieren bzw. diese leer sein, dann sollen zum Start des Programms 3-5 Mitglieder von euch generiert werden,  die der Benutzer sich mit "[2] Alle Benutzer anzeigen" anzeigen lassen kann.

#### 🔹 Erweiterung:

-Als nächste Aufgabe kannst du die Anwendung unter Verwendung von [MVVM](https://de.wikipedia.org/wiki/Model_View_ViewModel "https://de.wikipedia.org/wiki/model_view_viewmodel") neu Entwickeln. Auch in *Winforms*, [hier](https://devblogs.microsoft.com/dotnet/winforms-cross-platform-dotnet-maui-command-binding/ "https://devblogs.microsoft.com/dotnet/winforms-cross-platform-dotnet-maui-command-binding/") kann man sich inspirieren lassen. 
-Anstelle des JSON Ein- und Auslesen werden Mitglieder in einer [SQLiteDB](https://www.nuget.org/packages/Microsoft.Data.Sqlite "https://www.nuget.org/packages/microsoft.data.sqlite") gespeichert.
-Benutzer können angelegt, bearbeitet und gelöscht werden.


###
[[Startseite]]





