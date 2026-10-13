# synapsESP – Eurorack ESP32 Control Module

synapsESP ist ein quelloffenes Eurorack-Modul auf Basis des ESP32-Microcontrollers, entwickelt für die flexible Steuerung, Generierung und Verarbeitung von Audio- und CV-Signalen in einem Eurorack-Synthesizer-System.

---

## Features

* ESP32 Core: Leistungsstarke Steuerung für digitale Generierung, DSP und Schnittstellen.
* Display & UI-Integration: Schnittstellen für Displays (z. B. ILI9341 Touch-Display) sowie dedizierte UI-Bedienelemente.
* CV & Audio I/O: Ein- und Ausgänge zur Handhabung von Steuerspannungen (CV) und Audiosignalen im Eurorack-Standard.
* Spannungsversorgung: Standard Eurorack Power-Anschluss mit integrierter Schutzbeschaltung.

---

## Projektstruktur

synapsESP/
├── audio.kicad_sch        # Schaltplan: Audio I/O
├── cv.kicad_sch           # Schaltplan: CV-Eingänge/Ausgänge
├── io.kicad_sch           # Schaltplan: Allgemeine E/A & Peripherie
├── power.kicad_sch        # Schaltplan: Stromversorgung & Schutz
├── ui.kicad_sch           # Schaltplan: Benutzeroberfläche / Bedienelemente
├── esp32.kicad_pcb        # KiCad PCB Layout
├── esp32.kicad_pro        # KiCad Hauptprojekt
├── Display_ILI9341.*      # Symbol- & Footprint-Bibliotheken für das Display
└── .gitignore             # Git-Ausschlusskriterien für temporäre KiCad-Dateien

---

## Hardware & Design

Das Modul wurde in KiCad strukturiert und modular aufgebaut. Es teilt die unterschiedlichen Blöcke (Audio, CV, UI, Power) in übersichtliche Schaltplan-Hierarchien auf.

### Voraussetzungen / Design-Tools

* KiCad (Empfohlen: v7 oder neuer)
* Passende Bibliotheken für Gehäuse-/Panel-Abmessungen und Spezialkomponenten (z. B. Display-Module)

---

## Inbetriebnahme & Git

Um das Projekt lokal zu klonen:

git clone https://github.com/hanebuechenes/synapsESP.git

Öffne anschließend die Datei esp32.kicad_pro in KiCad, um den Schaltplan zu lesen oder das PCB-Layout anzupassen.

---

## Lizenz

Dieses Projekt ist unter der CERN Open Hardware Licence / MIT License veröffentlicht (frei zur persönlichen Nutzung und Modifikation).
