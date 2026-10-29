# Bankroll – Poker & Casino

Die Bankroll-App als Web-App (PWA), die man auf dem iPhone auf den Home-Bildschirm legen kann.
Sie startet im Vollbild wie eine normale App, funktioniert auch offline und speichert alle Einträge direkt auf dem Gerät.

## Online stellen (GitHub Pages)

1. Diesen Branch in `main` mergen.
2. Auf GitHub: **Settings → Pages → Build and deployment → Source: «Deploy from a branch»**, Branch `main`, Ordner `/ (root)`, speichern.
   GitHub Pages für private Repos braucht GitHub Pro – sonst das Repo auf **Public** stellen (deine Daten liegen nie im Repo, nur auf dem iPhone).
3. Nach ca. 1 Minute ist die App unter `https://noray57.github.io/Bankroll/` erreichbar.

## Auf den Home-Bildschirm legen

1. Die Adresse auf dem iPhone in **Safari** öffnen.
2. Unten auf **Teilen** (Quadrat mit Pfeil) tippen.
3. **«Zum Home-Bildschirm»** wählen → **Hinzufügen**.

## Daten aus dem alten Artefakt übernehmen

1. Im Bankroll-Artefakt auf claude.ai: **Verlauf → CSV kopieren**.
2. In der App: **Verlauf → Daten importieren**, einfügen, **Importieren**.

Doppelte Einträge werden beim Import automatisch übersprungen.

## Datensicherung

Die Einträge liegen nur auf dem jeweiligen Gerät. Unter **Verlauf → CSV-Datei sichern** kannst du ab und zu eine Sicherung in «Dateien» oder per Mail ablegen und sie bei Bedarf wieder importieren.

## Dateien

- `index.html` – die ganze App
- `manifest.webmanifest`, `icons/` – App-Name und Icon für den Home-Bildschirm
- `sw.js` – Offline-Cache (bei Änderungen `CACHE`-Version erhöhen)
