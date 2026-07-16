# CowCare — One-Pager

Marketing-One-Pager für **CowCare**, das kamerabasierte KI-System für Milchviehbetriebe.
Statische Seite (ein `index.html`, keine Build-Tools), gehostet über GitHub Pages.
Fokus: **Pilot-Farmer-Recruiting** (5 Plätze, UK + DE) + **Investoren** (Seed-Runde).

## Live

https://weconn3ct.github.io/cowcare/

## Platzhalter, die noch getauscht werden müssen

Beide stehen zentral am Anfang des `<script>`-Blocks in `index.html`:

| Konstante | Aktuell | Was tun |
|---|---|---|
| `CALENDLY_URL` | `'PLACEHOLDER'` | Echten Calendly-Link eintragen — solange Platzhalter, zeigt die Investor-Sektion eine „Terminbuchung folgt in Kürze"-Box; mit echtem Link lädt automatisch das Calendly-Widget |
| `INVESTOR_EMAIL.en` | `'PLACEHOLDER'` | Englische Investoren-Adresse eintragen — bis dahin fällt der EN-mailto auf `info@weconn3ct.de` zurück |

Investoren-Mail DE: `info@weconn3ct.de` (fest eingetragen).

## Formular (Pilot-Bewerbung)

Läuft über FormSubmit an `mentor.sadiku@weconn3ct.de` — beim **ersten** Absenden schickt FormSubmit eine Bestätigungs-Mail an diese Adresse (einmal bestätigen, danach kommen Bewerbungen an).

## Sprache

Deutsch/Englisch mit Umschalter. Automatik: deutsche Browser → DE, alle anderen → EN. Manuelle Wahl wird in localStorage gespeichert.

## Design & Inhalte

- Farben & Styling nach CowCare-Pitchdeck (Forest-Green, Orange-Akzent, Poppins/Figtree), Bilder aus dem Deck extrahiert (`assets/`)
- Inhaltliches Konzept: [docs/superpowers/specs/2026-07-16-pilot-investor-relaunch-design.md](docs/superpowers/specs/2026-07-16-pilot-investor-relaunch-design.md)
