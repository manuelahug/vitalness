# Vitalness – Website

Neue Website für [vitalness.ch](https://www.vitalness.ch) – Bioresonanz-Therapie, Massagen und komplementäre Behandlungen in Muhen bei Aarau (Gabriella Hug).

Ersetzt die bisherige Wix-Seite. Statisches HTML/CSS ohne Build-System – direkt hostbar auf GitHub Pages, Cloudflare Pages oder jedem beliebigen Webhosting.

## Struktur

- Jede Seite liegt als `ordner/index.html` vor → saubere URLs (`/bioresonanztherapie/`, `/massagen/`, …)
- Die URL-Slugs entsprechen der alten Wix-Seite (SEO-Kontinuität beim Domain-Umzug)
- `css/style.css` – zentrales Stylesheet (Design-System mit CSS-Variablen)
- `sitemap.xml`, `robots.txt`, `404.html` – SEO/Hosting-Basics
- Schriften via [fonts.bunny.net](https://fonts.bunny.net) (datenschutzfreundlich, kein Google-Tracking)
- Keine Cookies, kein Tracking, kein JavaScript nötig

## Seiten

Start, Angebot (Übersicht + 7 Behandlungsseiten), Preisliste, Referenzen, Über mich, Kontakt, Impressum, Datenschutz.

## Lokal ansehen

```bash
python3 -m http.server 8734
```

Dann <http://localhost:8734> öffnen.

## Deployment

GitHub Pages, Branch `main`, Root-Verzeichnis. Sobald die Domain von Wix wegzieht:
`CNAME`-Datei mit `www.vitalness.ch` ins Root legen und DNS auf GitHub Pages zeigen.
