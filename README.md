# FocusLock – Stop Doomscrolling 🛑

FocusLock ist eine leistungsstarke, minimalistische Browser-Erweiterung, die entwickelt wurde, um ablenkende Websites gezielt zu blockieren und sogenanntes "Doomscrolling" zu stoppen. Die Erweiterung nutzt einen psychologischen "Friction"-Mechanismus (gewollte Verzögerung), um impulsive Surfgewohnheiten zu durchbrechen und deine Produktivität aktiv zu schützen.

## ✨ Hauptfunktionen

*   **Intelligentes Blocking:** Blockiere komplette Domains (z.B. `reddit.com`) oder spezifische Pfade (z.B. `youtube.com/shorts`). Single-Page Applications (SPAs) werden dabei dynamisch in Echtzeit unterstützt.
*   **Psychologische Friction:** Gewollte Wartezeiten (z.B. 5 Sekunden) beim Versuch, eine blockierte Seite ("Snooze") aufzurufen, verhindern das automatische, unbewusste Vorbeiklicken an der Sperre. 
*   **Zeitkontingente (Quotas):** Lege tägliche, wöchentliche oder stündliche Budgets für ablenkende Webseiten fest (z.B. max. 20 Min. Social Media am Tag). Nach Ablauf sperrt sich die Seite rigoros.
*   **Snooze-System:** Erlaube dir im Notfall kontrollierte, kurze Ausnahmen (+10 Sekunden, +1 Min, +5 Min) – unter ständiger, visueller Beobachtung durch den Block-Timer.
*   **Detaillierte Statistiken:** Verfolge deine Browsing-Zeit auf und vergleiche deine Aktivitäten der letzten 30 Tage ein einem aufgeräumten Dashboard direkt im Popup.
*   **Premium Design:** Eine zusammengefasste, minimalistische Benutzeroberfläche (Single-Popup) im "Fintech-Style" (dunkler Text, weißer Hintergrund, leuchtend grüner Akzent).
*   **100 % Privat & Offline:** Alle Daten (Regeln, Einstellungen, Statistiken) werden ausschließlich auf deinem Endgerät lokal gespeichert (`chrome.storage.local`). Es gibt keine Tracker, Analytics oder Remote-Server.

## 🚀 Installation (Manuell / Entwicklermodus)

Da FocusLock hier als roher Codeback vorliegt, kannst du es mühelos als "Entpackte Erweiterung" in allen Chromium-basierten Browsern (Google Chrome, Microsoft Edge, Brave, Vivaldi) installieren:

1. Lade das Projekt herunter oder klone das Repository lokal auf deinen PC.
2. Öffne in deinem Browser die Erweiterungsverwaltung:
   * Chrome/Brave: `chrome://extensions/`
   * Edge: `edge://extensions/`
3. Aktiviere den **Entwicklermodus** (befindet sich als Schiebeschalter meist oben rechts).
4. Klicke auf den Button **"Entpackte Erweiterung laden"** (Load unpacked).
5. Wähle den `extension`-Ordner aus (in welchem sich die Datei `manifest.json` befindet).
6. 🎉 FocusLock ist nun installiert! Am besten pinnst du dir das Icon oben rechts in der Browser-Leiste an, um direkten Zugriff auf die Oberfläche zu haben.

## 💻 Technologie-Stack

FocusLock ist extrem rasend und schlank aufgebaut und verzichtet komplett auf riesige JS-Frameworks zugunsten maximaler Performance.

*   **Manifest V3** API-Architektur (moderner Standard für Chrome-Erweiterungen).
*   **Vanilla JavaScript (ES6+)** für extrem schnelle Hintergrunddienste (Service Worker) und Inhaltsinjektionen (Content Scripts).
*   **Vanilla CSS3** inkl. CSS-Variablen für ein flexibles und wunderschönes Design-System.
*   **Abhängigkeiten:** Keine externen JavaScript-Pakete oder NPM-Abhängigkeiten. (Die Benutzeroberfläche lädt lediglich aus designtechnischen Gründen Google Fonts ("DM Sans") und Material Icons über offizielle Server).

## 🔒 Datenschutz & Architektur

*   **Datenschutz:** Deine Privatsphäre steht an erster Stelle. Einen detaillierten Überblick darüber, warum überhaupt welche Berechtigungen angefordert werden und warum das System 100 % sicher läuft, findest du im Formular [datenschutz.md](./datenschutz.md).
*   **Architektur:** Wenn du Entwickler bist und die exakte Code-Basis verstehen möchtest – inklusive Designvorgaben und Kernlogik – sieh dir gerne die angelegte Blaupause [project.md](./project.md) an.
