# Lab 1: Initialer Prompt für die To-Do Web-App

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


# Lab 2: Erstellen einer neuen Funtion
Prompt, Übersetzt ins Deutsche:

```
Füge eine Drag-and-Drop-Funktionalität für die Aufgabenkarten im Kanban-Dashboard hinzu, um deren Status zu ändern.
```

Original Prompt:

Add drag and drop functionality to the task cards on the Kanban dashboard to change status

# Lab 3: Kiro Agent Hooks (Automatismen)

Prompt, Übersetzt ins Deutsche:

```
Erstelle einen Hook, der ausgelöst wird, wenn ich TypeScript- oder TSX-Dateien im To-Do-Projekt speichere. Er soll Codemuster und eine korrekte Fehlerbehandlung prüfen sowie Verbesserungsvorschläge machen. Verwende das fileEdited-Event mit Patterns für *.ts- und *.tsx-Dateien.
```

Original Prompt:

Create a hook that triggers when I save TypeScript or TSX files in the To-Do project. It should check code patterns, proper error handling, and suggest improvements. Use the fileEdited event with patterns for *.ts and *.tsx files.

Alternativ ist auch die automatische, im weiteren Verlauf immer aktualisierte Erstellung von Dokumentation.

Zuerst benötigen wir einen Initialen Prompt:
```
Falls noch nicht vorhanden, erstelle ein Verzeichnis doc/ . Darin erstelle eine Datei Todo-List_v1.md, die den bisherigen Projekt
Fortschritt dokumentiert. Erstelle im gleichen Verzeichnis eine Datei Todo-List_EN_v1.md, die die Dokumentation auf Englisch enthält.
```

Nun der Prompt, der den Kiro Hook erzeugt:
```
Wann immer die deutsche Dokumentation geändert wird, übernimm diese Änderungen auch ins englische Dokument.
```

# Lab 4: Steering Dokumente

Referenz: https://catalog.us-east-1.prod.workshops.aws/workshops/c485498c-eb35-4d8f-9412-26f9717ad365/en-US/steering/generate-steering-documents 

UX Steering Dokument Inhalt, übersetzt ins Deutsche:
```
UX- & Design-Richtlinien — AWS-Farbpalette
Farbpalette (Basierend auf der AWS-Marke)

    Primär (Aktionen & Highlights): #0972D3 (AWS Cloudscape Blue) — Buttons, Links, aktive Zustände

    Sekundär (Akzente & Hover): #FF9900 (AWS Orange) — Hover-Effekte, Highlight-Elemente, Call-to-Action

    Dunkel (Header & Navigation): #252F3E (AWS Squid Ink) — Navbar, Sidebar, Footer-Hintergründe

    Hohe Priorität / Dringend: #D91515 (AWS Red) — Überfällige Aufgaben, Fehlerzustände, Indikatoren für hohe Priorität

    Mittlere Priorität / Achtung: #FF9900 (AWS Orange) — Nahende Fristen, mittlere Priorität

    Niedrige Priorität / Erfolg: #037F0C (AWS Green) — Erledigte Aufgaben, Erfolgszustände, niedrige Priorität

    Hintergrund: #FAFAFA (Hellgrau) — Seitenhintergrund für klaren Kontrast

    Karten & Oberflächen: #FFFFFF (Weiß) — Kartenhintergründe mit dezentem Schatten

Visuelles Design

    Nutze ein sauberes, minimales Interface mit viel White Space

    Abgerundete Ecken (border-radius: 8px) für Karten und Buttons

    Schriftart: System-Font-Stack für Performance (system-ui, -apple-system, sans-serif)

    Kartenschatten: 0 1px 4px rgba(0, 0, 0, 0.1) für dezente Tiefe

Aufgabenkarten (Task Cards)

    Priorität als farbiger linker Rand auf jeder Karte (4px solid, basierend auf den obigen Prioritätsfarben)

    Tags als kleine farbige Badges mit abgerundeten Ecken anzeigen

    Fälligkeitsdatum mit visueller Dringlichkeit (Rot bei Verzug, Orange bei Fälligkeit heute, Grau für die Zukunft)

    Aktionen (Bearbeiten, Löschen, Erledigen) als Icon-Buttons, die bei Hover sichtbar werden

    Status-Badges: „To Do“ in Squid Ink, „In Progress“ in AWS Blue, „Completed“ in AWS Green

Barrierefreiheit (Accessibility)

    Alle interaktiven Elemente müssen per Tastatur navigierbar sein

    Verwendung von semantischem HTML (main, nav, section, article)

    Kontrastverhältnis von mindestens 4,5:1 für Text einhalten

    Aria-Labels für reine Icon-Buttons hinzufügen

    Fokus-Indikatoren müssen sichtbar sein (AWS Blue Outline verwenden)
```

