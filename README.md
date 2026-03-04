# Übersicht

Dieses Projekt ist eine **Windows-Desktopanwendung** (WinForms) auf Basis von **.NET Framework 4.7.2**.  
Es ermöglicht das **Erzeugen** und **Lösen** des klassischen **n‑Puzzle** (Schiebepuzzle, z. B. 8‑Puzzle / 15‑Puzzle) mit verschiedenen Suchverfahren und Heuristiken. Ergebnisse und Laufzeit-/Suchmetriken werden in der Oberfläche angezeigt.

# Funktionen

- Erzeugt neue n‑Puzzle-Spielfelder in mehreren Größen
- Löst Puzzles mit wählbaren Methoden (abhängig vom Projektumfang), z. B.:
  - A* (A-Star)
  - IDA* (Iterative Deepening A*)
  - Bidirektional / BA* (falls im Projekt vorhanden)
- Unterstützt auswählbare Heuristiken (falls vorhanden), z. B.:
  - Hamming
  - Manhattan-Distanz
  - Linear Conflict
  - Pattern Database (PDB) (benötigt PDB-Dateien)
- Zeigt Auswertung/Metriken an, u. a.:
  - benötigte Zeit
  - Lösungstiefe
  - Anzahl besuchter Knoten/Zustände
  - Speicherverbrauch (falls gemessen/ausgegeben)
- Optional: Experiment-/Testfenster zum Vergleichen von Heuristiken/Methoden (falls enthalten)

# Installation (Windows + Visual Studio)

Folge diesen Schritten, um das Projekt einzurichten und zu starten:

1. **Voraussetzungen installieren**
   - Windows 10/11
   - **Visual Studio 2019 oder Visual Studio 2022**
   - **.NET Framework 4.7.2 Developer Pack** (wichtig zum Bauen von `net472`)

2. **Quellcode beziehen**
   - Repository klonen oder als ZIP herunterladen und entpacken.

3. **Solution öffnen**
   - Die `*.sln` Datei in Visual Studio öffnen.

4. **Wiederherstellen / Build**
   - Visual Studio stellt Pakete meist automatisch wieder her.
   - Build über: **Build → Build Solution**

# Verwendung

1. In Visual Studio das richtige Startprojekt setzen:
   - Solution Explorer → Rechtsklick auf das WinForms-Projekt → **Als Startprojekt festlegen**


2. In der Anwendung:
   - Puzzle generieren (Größe auswählen)
   - Heuristik auswählen (falls verfügbar)
   - Lösungsmethode auswählen
   - Solver starten und Metriken sowie Zielzustand ansehen

# Ausgabe

Je nach Projektkonfiguration erfolgt die Ausgabe hauptsächlich in der UI:

- **Ziel-/Endzustand** wird visuell angezeigt
- **Ergebnisse / Statistiken** wie z. B.:
  - Laufzeit (ms)
  - Lösungstiefe
  - Anzahl besuchter Knoten
