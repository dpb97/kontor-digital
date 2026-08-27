# Kontor Digitalisierung

Marketing-Landingpage für **Kontor Digitalisierung & KI-Beratung** –
Digitalisierungs- und KI-Beratung für Maschinenbau- und
Fertigungsunternehmen im Mittelstand, gebaut mit
[Hugo](https://gohugo.io/) + [Tailwind CSS](https://tailwindcss.com/).

Teilt Design-System (Farben, Fonts, Layout-Stil) mit
[kontor-erp](https://github.com/dpb97/kontor-erp), ist aber ein
eigenständiges Angebot und eigenständiges Repo.

## Lokal starten

```bash
npm install
npm run build:css   # einmalig, oder erneut nach Klassen-Änderungen in layouts/
hugo server
```

## Build

```bash
npm run build:css
hugo --minify
```

Das Deployment nach GitHub Pages läuft automatisch über
`.github/workflows/hugo-pages.yml` bei jedem Push auf `main` (Node-Build
für die CSS, dann Hugo-Build). Damit das greift, muss unter
*Settings → Pages* als Quelle **GitHub Actions** eingestellt sein.
Live-URL: https://dpb97.github.io/kontor-digital/

Impressum/Datenschutz sind eigenständige deutsche Rechtstexte, analog zu
`kontor-erp`.
