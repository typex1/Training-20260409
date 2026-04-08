Lab 1:

Prompt in German:
Hier ist die Übersetzung deiner Projektbeschreibung ins Deutsche:

---

## Projektbeschreibung: Task-Management (To-Do) Web-App

Erstelle eine Task-Management-Webanwendung mit der folgenden Struktur:
```
Projektbeschreibung: Task-Management (To-Do) Web-App

Erstelle eine Task-Management-Webanwendung mit der folgenden Struktur:
Benutzeroberfläche (Single Page + Modals)

Dashboard mit:

    Aufgabenliste: Organisiert nach Status (To Do, In Progress, Completed) in Spalten im Kanban-Stil.

    Beispieldaten: 10 vorinstallierte Beispielaufgaben.

    Visuelle Elemente: Emojis für Kategorien und Prioritätsindikatoren (Hoch 🔴, Mittel 🟡, Niedrig 🟢).

    Aufgabenzähler: Anzeige nach Status (erledigt vs. ausstehend).

    „Neue Aufgabe“-Button: Gut sichtbar im oberen Bereich platziert.

    Aufgabenkarten: Jede Karte zeigt Titel, Kategorie, Priorität, Fälligkeitsdatum und Aktionsschaltflächen (Bearbeiten, Löschen, Status ändern).

Modal für Erstellung/Bearbeitung:

    Felder: Titel, Beschreibung, Priorität (Hoch/Mittel/Niedrig), Kategorie, Fälligkeitsdatum.

    Wiederverwendbarkeit: Dasselbe Modal wird sowohl für das Erstellen als auch für das Bearbeiten genutzt.

Aufgabendetails-Modal (bei Klick auf Karte):

    Anzeige der vollständigen Beschreibung, Fälligkeitsdatum, Priorität und Kategorie.

    Button „Als erledigt markieren“.

    Button „Löschen“ (mit Sicherheitsabfrage).

    Notiz-/Kommentarbereich: Eingabefeld für neue Kommentare sowie eine Liste mit Beispielkommentaren.

Bestätigungsdialog: Sicherheitsabfrage vor dem endgültigen Löschen einer Aufgabe.
Architektur (3-Schichten-Modell)

    Frontend: React mit funktionalen Formularen für vollständige CRUD-Operationen.

    Backend: Node.js mit einer REST-API (Endpunkte zum Erstellen, Lesen, Aktualisieren und Löschen von Aufgaben und Kommentaren).

    Datenbank: Buns native SQLite-Lösung (bun:sqlite) – keine externen Datenbank-Abhängigkeiten; Tabellen für Aufgaben, Kategorien, Prioritäten und Kommentare.

Runtime (Laufzeitumgebung)

Verwende Bun als Runtime und Paketmanager für das gesamte Projekt. Nutze das integrierte bun:sqlite für die lokale Datenspeicherung, um ohne einen externen Datenbankserver auszukommen.
```

Mit Formatierung:

### Benutzeroberfläche (Single Page + Modals)

**Dashboard mit:**
* **Aufgabenliste:** Organisiert nach Status (To Do, In Progress, Completed) in Spalten im **Kanban-Stil**.
* **Beispieldaten:** 10 vorinstallierte Beispielaufgaben.
* **Visuelle Elemente:** Emojis für Kategorien und Prioritätsindikatoren (Hoch 🔴, Mittel 🟡, Niedrig 🟢).
* **Aufgabenzähler:** Anzeige nach Status (erledigt vs. ausstehend).
* **„Neue Aufgabe“-Button:** Gut sichtbar im oberen Bereich platziert.
* **Aufgabenkarten:** Jede Karte zeigt Titel, Kategorie, Priorität, Fälligkeitsdatum und Aktionsschaltflächen (Bearbeiten, Löschen, Status ändern).

**Modal für Erstellung/Bearbeitung:**
* **Felder:** Titel, Beschreibung, Priorität (Hoch/Mittel/Niedrig), Kategorie, Fälligkeitsdatum.
* **Wiederverwendbarkeit:** Dasselbe Modal wird sowohl für das Erstellen als auch für das Bearbeiten genutzt.

**Aufgabendetails-Modal (bei Klick auf Karte):**
* Anzeige der vollständigen Beschreibung, Fälligkeitsdatum, Priorität und Kategorie.
* Button „Als erledigt markieren“.
* Button „Löschen“ (mit Sicherheitsabfrage).
* **Notiz-/Kommentarbereich:** Eingabefeld für neue Kommentare sowie eine Liste mit Beispielkommentaren.

**Bestätigungsdialog:** Sicherheitsabfrage vor dem endgültigen Löschen einer Aufgabe.

---

### Architektur (3-Schichten-Modell)

* **Frontend:** React mit funktionalen Formularen für vollständige **CRUD-Operationen**.
* **Backend:** Node.js mit einer **REST-API** (Endpunkte zum Erstellen, Lesen, Aktualisieren und Löschen von Aufgaben und Kommentaren).
* **Datenbank:** Buns native SQLite-Lösung (`bun:sqlite`) – keine externen Datenbank-Abhängigkeiten; Tabellen für Aufgaben, Kategorien, Prioritäten und Kommentare.

---

### Runtime (Laufzeitumgebung)

Verwende **Bun** als Runtime und Paketmanager für das gesamte Projekt. Nutze das integrierte **`bun:sqlite`** für die lokale Datenspeicherung, um ohne einen externen Datenbankserver auszukommen.


Lab 2 Prompt, Übersetzt ins Deutsche:

```
Füge eine Drag-and-Drop-Funktionalität für die Aufgabenkarten im Kanban-Dashboard hinzu, um deren Status zu ändern.
```

Original:
Add drag and drop functionality to the task cards on the Kanban dashboard to change status

