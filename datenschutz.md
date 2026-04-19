# Datenschutzerklärung für FocusLock

Der Schutz Ihrer Daten und Ihrer Privatsphäre hat bei FocusLock höchste Priorität. Diese Datenschutzerklärung erklärt transparent, welche Informationen bei der Nutzung der Browser-Erweiterung verarbeitet werden, wie sie gespeichert werden und warum wir spezifische Berechtigungen benötigen.

## 1. Datenerhebung

FocusLock erfasst Daten ausschließlich zu dem Zweck, die beworbene Kernfunktionalität (Blockierung von Webseiten und Zeiterfassung) bereitzustellen. Folgende Daten werden lokal während der Nutzung verarbeitet:

*   **Besuchte URLs und Domains:** Um zu prüfen, ob die aktuell aufgerufene Website auf Ihrer persönlichen Blockliste steht.
*   **Browsing-Verlauf und Nutzungsstatistiken:** Die Erweiterung erfasst die verbrachte Zeit auf Domains, um Ihnen Statistiken über Ihr Surfverhalten und die Nutzung von "Pausen" (Snoozes) der letzten 30 Tage anzuzeigen.
*   **Persönliche Konfigurationen:** Ihre individuell definierten Blockier-Regeln, Zeitlimits (Kontingente) und Einstellungen.

**Wichtig:** Es findet **kein Tracking** des gesamten Surfverhaltens über von Ihnen nicht besuchte Seiten hinweg zu Werbezwecken statt, und es werden keine persönlichen Identifikationsmerkmale (wie Name oder E-Mail) erhoben.

## 2. Datenspeicherung – 100 % Lokal

Ihre Privatsphäre ist durch unsere Architektur garantiert:

*   **Ausschließliche lokale Speicherung:** Alle erfassten Daten (inklusive Ihrer URLs, Einstellungen und Statistiken) werden **ausschließlich lokal auf Ihrem Endgerät** über die sichere Browser-Schnittstelle `chrome.storage.local` gespeichert.
*   **Keine externen Server:** **Es findet zu keinem Zeitpunkt eine Übertragung Ihrer Nutzerdaten oder Ihres Surfverhaltens an externe Server, Entwickler oder Dritte statt.** FocusLock arbeitet völlig eigenständig und datenschutzfreundlich.

## 3. Notwendige Berechtigungen

Um ordnungsgemäß zu funktionieren, erfordert FocusLock bestimmte Browser-Berechtigungen. Wir fordern nur das absolute Minimum an Berechtigungen an:

| Berechtigung | Technischer Zweck |
| :--- | :--- |
| **`tabs`** | Notwendig, um die URL des aktiven Tabs auszulesen, damit das System abgleichen kann, ob die besuchte Seite den von Ihnen definierten Blockregeln entspricht. |
| **`storage`** | Essentiell, um Ihre Einstellungen, Ausnahmeregeln und lokalen Zeitstatistiken permanent auf Ihrer Festplatte (`chrome.storage.local`) zu speichern. |
| **`scripting`** | Wird benötigt, um das FocusLock-Sperr-Overlay und die dazugehörige Blockier-Logik direkt in die zu sperrenden Webseiten einzufügen. |
| **`alarms`** | Erforderlich für die Ausführung von Hintergrundprozessen im richtigen Takt, z. B. um regelmäßig die erfassten Browsing-Zeiten zu speichern. |
| **`webNavigation`** | Erlaubt es der Erweiterung, Navigationsereignisse (wie das Laden einer neuen Seite) sofort zu erkennen, um Injektionen optimal zu timen, besonders auf modernen "Single Page Applications" (SPA). |
| **`<all_urls>`** | *(Host-Berechtigung)* Zwingend erforderlich, damit die Erweiterung uneingeschränkt auf allen potenziellen Websites arbeiten kann, da Sie potenziell jede beliebige Domain blockieren können. |

## 4. Drittanbieter & externe Verbindungen

FocusLock ist grundsätzlich so konzipiert, dass externe Abhängigkeiten minimiert werden.

*   **Keine Tracker, keine Analytics:** Wir binden **keine** Drittanbieter-Analysetools (wie Google Analytics) oder Web-Tracker ein. Es wird kein separates Nutzerverhalten durch Dritte gemessen.
*   **Gestaltungsmittel (CDNs):** Das sichtbare User-Interface der Erweiterung lädt standardisierte Web-Schriftarten (*Google Fonts: DM Sans*) und Icons (*Material Icons*) dynamisch von offiziellen Content Delivery Networks (CDNs), um die Darstellung einwandfrei abzubilden. Dabei sendet Ihr Browser systembedingt eine gewöhnliche Anfrage an diese Server.

## 5. Ihre Nutzerkontrolle

Sie haben die volle und uneingeschränkte Kontrolle über Ihre Daten:

*   **Daten-Export/Import:** Sie können in den Einstellungen Ihre gesammelten lokalen Statistiken und Regeln manuell im JSON-Format exportieren und jederzeit wiederherstellen.
*   **Daten löschen durch Deinstallation:** Da alle Daten ausschließlich lokal in den Speicherbereichen Ihres Browsers abgelegt sind, werden **durch eine einfache Deinstallation von FocusLock sämtliche gesammelten Daten (Statistiken, Einstellungen und Regeln) restlos und unwiderruflich von Ihrem Gerät gelöscht**. Es verbleiben keine Restdaten bei uns oder auf Servern im Internet.
