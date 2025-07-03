

###🔹 Allgemeine Coding Challenges

- [LeetCode](https://leetcode.com/): Eine beliebte Plattform zum Üben von Programmieraufgaben, besonders für technische Bewerbungsgespräche und algorithmisches Denken.

- [Coding Dojo Katas](https://codingdojo.org/kata/)Eine Sammlung von kleinen, wiederholbaren Programmierübungen („Katas“) zur Verbesserung von Codequalität und Problemlösungsfähigkeiten.

- [Clean Code Developer – Coding Dojo](https://ccd-school.de/coding-dojo/): Eine deutschsprachige Plattform mit Fokus auf sauberen Code und Softwarehandwerk, inklusive Dojos zum Üben guter Programmierpraktiken.
- 

---

#🔹 Übungsprojekt Mitgliedervewaltungssoftware (in mehrere Abschnitte aufgeteilt)

## 🟢 **Stufe 1: Grundlagen – Klassen und Objekte**

**Ziel:** Einführung in Klassen, Attribute und Objektinstanzen.

- Erstelle eine Klasse `Mitglied` mit den Attributen:
  - `id` (zunächst manuell vergeben)
  - `name`
  - `alter`
  - `mitgliedsstatus`
- Erstelle 2–3 Objekte dieser Klasse im Code.
- Gib Name und Mitgliedsstatus dieser Mitglieder in der Konsole aus.

➡️ **Lernziel:** Klassen, Konstruktor, Attribute, Objektinstanzen, einfache Konsolenausgabe.

---

## 🟡 **Stufe 2: Vergleich und Kategorisierung**

**Ziel:** Einführung in Bedingungen, Listen und einfache Logik.

- Speichere alle Mitglieder in einer Liste.
- Prüfe, ob es doppelte Mitglieder gibt (gleicher Name, Alter, Status).
- Gib Mitglieder nach Alterskategorie aus:
  - Kinder: unter 13
  - Teenager: 13–19
  - Erwachsene: 20+

➡️ **Lernziel:** Listen, Schleifen, Bedingungen, Vergleichslogik.

---

## 🟠 **Stufe 3: Konsolenmenü und Benutzerinteraktion**

**Ziel:** Einführung in Benutzereingaben und einfache Menüs.

- Erstelle ein Menü mit:
  - `[1]` Neues Mitglied hinzufügen
  - `[2]` Alle Mitglieder anzeigen
  - `[10]` Beenden
- Eingabe aller Attribute über Konsole (ID noch manuell)

➡️ **Lernziel:** `input()`, Schleifen, einfache Menüführung.

---

## 🔵 **Stufe 4: Automatische ID-Vergabe und Validierung**

**Ziel:** Einführung in Validierung und Fehlerbehandlung.

- `ID` wird automatisch vergeben (z. B. mit einem Zähler).
- Validierung:
  - Name: nur Buchstaben, mindestens 3 Zeichen
  - Alter: muss eine Zahl sein
- **Bonus:** Wiederhole Eingabe bei Fehlern.

➡️ **Lernziel:** Fehlerbehandlung (`try/except`), benutzerdefinierte Fehlermeldungen, Validierung.

---

## 🟣 **Stufe 5: JSON-Speicherung**

**Ziel:** Einführung in Dateispeicherung und JSON.

- Menü erweitern:
  - `[3]` Mitglieder als JSON speichern
  - `[4]` Mitglieder aus JSON laden
- Speicherort z. B. `mitglieder.json`

➡️ **Lernziel:** Dateioperationen, JSON, Serialisierung/Deserialisierung.

---

## 🔴 **Stufe 6: Zufällige Mitglieder generieren**

**Ziel:** Einführung in zufällige Daten und Programmstart-Logik.

- Wenn keine JSON-Datei vorhanden oder leer:
  - Erzeuge 3–5 zufällige Mitglieder beim Start

➡️ **Lernziel:** `os.path`, Zufallsfunktionen, Startlogik.

---

## 🟤 **Erweiterung: GUI mit WinForms und SQLite (optional, fortgeschritten)**

**Ziel:** Einführung in GUI-Programmierung und Datenbanken.

- MVVM-Struktur
- SQLite statt JSON
- Mitglieder können bearbeitet und gelöscht werden

➡️ **Lernziel:** GUI-Design, Datenbankzugriff, MVVM-Architektur.

---





#🔹 Mitgliederverwaltungssoftware (Selbes Projekt am Stück)

> **Ziel:** Entwicklung einer Konsolenanwendung zur Verwaltung von Vereinsmitgliedern mit Fokus auf Datenvalidierung, Benutzerinteraktion, JSON-Handling und optionaler MVVM-Architektur mit SQLite.

## 🔧 Funktionen

Die Anwendung verwaltet Mitglieder mit folgenden Attributen:

- `Id` *(automatisch vergeben, eindeutig)*
- `Name` *(nur Buchstaben, mind. 3 Zeichen)*
- `Alter` *(gültige Zahl, mit benutzerdefinierter Fehlermeldung)*
- `Mitgliedsstatus` *(z. B. „Kassenwart“, „Mitglied“, etc.)*

Beispiel: `Bob, 29, Kassenwart`

### 📋 Funktionalitäten

- 🔍 Mitglieder anzeigen: Ausgabe von Name und Mitgliedsstatus
- 🧭 Duplikate finden: Mitglieder mit identischem Namen, Alter und Status erkennen → Ausgabe der `Id`
- 🧒👦🧑 Alterskategorien zählen:
  - Kinder: unter 13
  - Teenager: 13–19
  - Erwachsene: ab 20

## 🖥️ Konsolenmenü

- `[1]` Neuen Benutzer hinzufügen
- `[2]` Alle Benutzer anzeigen
- `[3]` Mitglieder als JSON speichern
- `[4]` Mitglieder aus JSON laden
- `[10]` Beenden

- ### ✅ Validierung & Fehlerbehandlung

- **Name**: nur Buchstaben, mind. 3 Zeichen
- **Alter**: muss eine gültige Zahl sein (mit Wiederholung bei Fehler)
- **Id-Vergabe**: automatisch, eindeutig
- **JSON-Datei**: frei wählbarer Name & Speicherort

## 🧪 Initialisierung & Testdaten

- Beim ersten Start (wenn keine JSON-Datei vorhanden oder leer):
  - Automatische Generierung von 3–5 zufälligen Mitgliedern
- Manuelles Anlegen von 2–3 Testobjekten im Code zur Überprüfung

## 🚀 Erweiterung: MVVM + SQLite

Für fortgeschrittene Umsetzung in einer GUI-Anwendung (z. B. mit WinForms oder .NET MAUI)

### Architektur: MVVM (Model-View-ViewModel)

- **Model**: Datenstruktur & Logik
- **ViewModel**: Bindings, Commands, Validierung
- **View**: Benutzeroberfläche (WinForms oder XAML)

### Datenbank statt JSON

- Speicherung der Mitglieder in einer SQLite-Datenbank
- Verwendung von `Microsoft.Data.Sqlite` (NuGet)
- CRUD-Funktionalitäten:
  - ➕ Anlegen
  - ✏️ Bearbeiten
  - ❌ Löschen

## 🧠 Zusätzliche Ideen

- 🔐 Login-System mit Rollen (Admin, Benutzer)
- 📊 Statistiken (z. B. Altersdurchschnitt, häufigste Mitgliedsrollen)
- 🌐 Web-API oder Blazor-Frontend
- 🧪 Unit-Tests für Validierung & Logik



-Als nächste Aufgabe kannst du die Anwendung unter Verwendung von [MVVM](https://de.wikipedia.org/wiki/Model_View_ViewModel "https://de.wikipedia.org/wiki/model_view_viewmodel") neu Entwickeln. Auch in *Winforms*, [hier](https://devblogs.microsoft.com/dotnet/winforms-cross-platform-dotnet-maui-command-binding/ "https://devblogs.microsoft.com/dotnet/winforms-cross-platform-dotnet-maui-command-binding/") kann man sich inspirieren lassen. 
-Anstelle des JSON Ein- und Auslesen werden Mitglieder in einer [SQLiteDB](https://www.nuget.org/packages/Microsoft.Data.Sqlite "https://www.nuget.org/packages/microsoft.data.sqlite") gespeichert.
-Benutzer können angelegt, bearbeitet und gelöscht werden.


###
[[Startseite]]





