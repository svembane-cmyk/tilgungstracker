# Tilgung. – Unterhaltstracker

Private, statische Web-App zum Erfassen von Unterhaltsrückständen, Zahlungen und zur Berechnung einer unverbindlichen Tilgungsprognose. Funktioniert auch offline nach dem ersten Besuch.

## Funktionen

- Restschuld und Tilgungsfortschritt (Cent-genau)
- Tilgung alter Rückstände getrennt vom laufenden Unterhalt
- Buchungen, Monatsübersicht, Korrekturen und Nachforderungen
- Prognose mit frei wählbarer Monatsrate und Startmonat
- JSON-Backup / -Import, CSV-Export
- iPhone-optimiert, als App zum Home-Bildschirm hinzufügbar

## Datenschutz

**Die Daten werden nur im lokalen Browser-Speicher (`localStorage`) auf dem jeweiligen Gerät gespeichert.** Es gibt keine Datenbank, keine Cloud-Synchronisierung und keine externe Analytik. Beträge und Buchungen werden nicht an GitHub übertragen. Beim Wechsel des Browsers, der Domain, des Geräts oder von der lokalen HTML-Datei zur GitHub-Pages-Adresse muss die Datenübertragung über **Einstellungen → Sicherung (JSON) → Sicherung importieren** erfolgen. Backup-Dateien enthalten vertrauliche Informationen und sollten nicht ins Repository hochgeladen werden. Der Code enthält bewusst keine persönlichen Standardbeträge.

**GitHub Pages-Webseiten können öffentlich erreichbar sein**, auch wenn dein Quellcode in einem privaten Repository liegt. Bei einem öffentlichen Repository kann auch jeder den Programmcode einsehen; persönliche Zahlungsdaten stehen dort nur, wenn du sie selbst hochlädst. Für einen privaten Online-Dienst mit geräteübergreifender Anmeldung wären zusätzliche Zugangskontrollen und Speicherung erforderlich.

## GitHub Pages veröffentlichen

1. Neues Repository `tilgungswracker` anlegen. Nicht mit vorhandenen anderen App-Repositories vermischen.
2. `index.html`, `sw.js`, `manifest.webmanifest`, `icon.svg`, `README.md` hochladen (oder diesen ZIP-Inhalt entpackt verwenden).
3. Unter **Settings → Pages → Build and deployment → Deploy from a branch** wählen, Branch `main` und Ordner `/(root)` setzen, speichern.
4. GitHub zeigt anschließend eine Pages-Adresse wie `https://DEINNAME.github.io/tilgungswracker/` an.
5. iPhone: Seite in Safari aufrufen, Teilen → Zum Home-Bildschirm.

## Finanzielle Einordnung

Die Modellrechnung setzt gleichbleibende Raten ohne neue Rückstände, Zinsen oder Gebühren voraus und ist keine amtliche Forderungsabrechnung. Bei Lohnpfändungen darf nur der tatsächlich auf den Altrückstand angerechnete Anteil als Tilgung erfasst werden.