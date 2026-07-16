# CowCare-Website v3 — Pilot-Recruiting + Investor-Signal

Datum: 2026-07-16 · Status: vom User freigegeben (Chat-Review, inkl. Ergänzung Entstehungsgeschichte)

## Ziel
Die Seite erklärt CowCare ehrlich (was existiert, was gerade passiert, wohin es geht) und hat zwei Conversions:
1. **Primär:** Farmer bewerben sich als Pilotbetrieb (Formular)
2. **Sekundär:** Investoren nehmen Kontakt auf (mailto + Calendly-Widget)

## Entscheidungen (gegrillt & bestätigt)
- **Zielgruppe:** Farmer primär (Hero + Haupt-CTA), Investoren eigene prominente Sektion
- **Ehrlicher Stand:** Tracking „entwickelt & auf realem Videomaterial validiert — bereit für den ersten Hof". KEIN „läuft im Feldeinsatz". Verhaltenserkennung wird jetzt mit Piloten trainiert.
- **Pilot-Deal:** komplett kostenlos (Installation/Hardware auf CowCare-Kosten), Hof teilt Videomaterial + Feedback; Gegenleistung: Dashboard ab Tag 1, Warnungen zuerst, dauerhafte Vorzugskonditionen
- **Umfang:** 5 Pilotplätze, UK + Deutschland
- **Seed-Runde:** erwähnen („Wir öffnen unsere Seed-Runde"), KEINE Beträge auf der Seite
- **Investor-CTA:** mailto (DE-Besucher → info@weconn3ct.de, EN-Besucher → Platzhalter-Adresse, wird noch eingerichtet) + Calendly-Inline-Widget mit Platzhalter-URL (zentrale Konstante; solange Platzhalter aktiv ist, zeigt die Box „Terminbuchung folgt in Kürze")
- **Preise:** nicht mehr als eigene Sektion — klein in der Investor-Sektion als „Geschäftsmodell nach dem Pilotprogramm", mit Hinweis auf Piloten-Vorzugskonditionen
- **Traction öffentlich:** NUR Sussex-Gewinn-Badge + University-of-Sussex-Forschung. KEINE Farmer-Zitate (nicht freigegeben).
- **Pilotdauer:** keine feste Zahl — „Trainingsphase über die Saison 2026/27"
- **Entstehungsgeschichte (Ergänzung):** Praveenan Mathew entwickelte in seiner Masterarbeit (University of Sussex) eine KI, die Kühe zuverlässig erkennt; gemeinsam mit WECONN3CT (KI- & Softwareentwicklung aus Deutschland) wurde daraus ein echtes Projekt. Mission: Landwirtschaft fördern — Technik für Tier, Mensch und Umwelt. Schön formuliert, eigene Sektion.

## Seitenstruktur
1. Nav: Warum · Lösung · Der Plan · Pilotprogramm · Investoren · FAQ + CTA „Pilotbetrieb werden"
2. Hero (Foto bleibt): Sussex-Badge, farmer-first Headline, Lead mit Pilot-Aufruf, CTAs [Pilotbetrieb werden][Für Investoren], Stats-Leiste (Stufe 1 ✓ / 5 Plätze / 0 Sensoren / £0 Kosten)
3. Problem (dunkel, bestehende Texte)
4. Lösung: 4 Säulen mit Status-Tags (Entwickelt ✓ / In Training / Beta / Geplant)
5. Der Plan: 3-Stufen-Roadmap, Stufe 2 hervorgehoben
6. Pilotprogramm: 3 Deal-Karten (bekommen/brauchen/Ablauf) + Bewerbungsformular (Name, E-Mail, Land, Herdengröße, Kameras vorhanden, Nachricht) via FormSubmit
7. Technologie (3 Schritte, bestehend, gekürzt)
8. Potenzial („Was die Forschung zeigt" — Zahlen mit Quellen als belegtes Ziel)
9. Entstehungsgeschichte („Aus einer Masterarbeit wurde eine Mission")
10. Investoren (dunkel): Momentum, Markt-Chips, Geschäftsmodell klein, mailto + Calendly
11. Team · 12. FAQ (Pilot-Fragen + „Wie kann ich investieren?") · 13. Footer

## Technik
- Weiterhin eine statische index.html, DE/EN via bestehendem i18n-System (alle neuen Strings in beiden Sprachen)
- Konfig-Konstanten am Script-Anfang: `CALENDLY_URL`, `INVESTOR_EMAIL = {de, en}`
- Raus: generisches Kontaktformular, eigenständige Preis-Sektion, Farmer-Zitate
