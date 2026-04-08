# Kiro-CLI Anwendungsbeispiele – Deutsche Bahn / Transportwesen

Kurze Beispiele zum Ausprobieren (jeweils ca. 5 Minuten).

---

## 1. Verspätungsanalyse aus CSV-Daten

```
Ich habe eine CSV-Datei "verspaetungen_q1.csv" mit den Spalten: Zugnummer, Linie, Abfahrt_Soll,
Abfahrt_Ist, Ankunft_Soll, Ankunft_Ist, Bahnhof. Erstelle ein Python-Skript, das:
- die durchschnittliche Verspätung pro Linie berechnet
- die Top-5-Bahnhöfe mit den meisten Verspätungen über 5 Minuten ausgibt
- ein einfaches Balkendiagramm als PNG speichert
```

---

## 2. Schichtplan-Generator für Lokführer

```
Schreibe ein Python-Skript, das einen Wochen-Schichtplan für 8 Lokführer generiert.
Bedingungen: maximal 8 Stunden pro Schicht, mindestens 11 Stunden Ruhezeit zwischen
zwei Schichten, jeder Lokführer hat mindestens 2 freie Tage pro Woche. Ausgabe als
übersichtliche Markdown-Tabelle.
```

---

## 3. Fahrplan-Daten in strukturiertes JSON umwandeln

```
Hier ist ein Auszug aus einem Fahrplan als Freitext:

"ICE 574 fährt ab Hamburg Hbf um 06:12, hält in Hannover Hbf (07:24), Göttingen (08:01),
Kassel-Wilhelmshöhe (08:22) und kommt in Frankfurt Hbf um 09:48 an."

Wandle diesen Text in ein strukturiertes JSON-Format um mit den Feldern: zugnummer, typ,
stationen (jeweils mit name und uhrzeit), abfahrt und ankunft. Erstelle außerdem eine
Python-Funktion, die beliebige Fahrplan-Texte in diesem Stil parsen kann.
```

---

## 4. Wartungsprotokoll-Vorlage erstellen

```
Erstelle eine Markdown-Vorlage für ein Wartungsprotokoll eines Schienenfahrzeugs (z.B. ICE 4).
Die Vorlage soll enthalten: Fahrzeugnummer, Baureihe, Datum der Inspektion, Prüfer,
Checkliste mit Kategorien (Bremsen, Türen, Klimaanlage, Stromabnehmer, Drehgestelle),
jeweils mit Status (OK / Mangel / Kritisch) und einem Bemerkungsfeld. Zusätzlich ein
Abschnitt für Folgemaßnahmen mit Priorität und Frist.
```

---

## 5. Einfache REST-API für Streckenstörungen

```
Erstelle mit Python (Flask) eine minimale REST-API für Streckenstörungen mit folgenden
Endpunkten:
- GET /stoerungen – alle aktuellen Störungen auflisten
- POST /stoerungen – neue Störung melden (Felder: strecke, art, beschreibung, seit)
- DELETE /stoerungen/<id> – Störung als behoben markieren
Nutze eine einfache In-Memory-Liste als Datenspeicher. Füge 3 Beispiel-Störungen als
Testdaten ein (z.B. "Oberleitungsstörung Strecke Köln-Düsseldorf").
```
