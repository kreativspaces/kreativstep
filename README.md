# kreativstep — Portfolio-Redesign

Statisches HTML/CSS-Redesign für kreativstep.de.

## Struktur
- `index.html` — Startseite (Hero + Vorschau)
- `portfolio.html` — vollständiges Portfolio-Grid
- `project.html` — Vorlage für Einzelprojekt-Seiten (kopieren & anpassen)
- `about.html` — Über mich
- `contact.html` — Kontakt
- `css/style.css` — alle Design-Tokens und Styles
- `js/main.js` — mobiles Navigationsmenü
- `img/` — Platzhalter-Ordner für eigene Bilder

## Bilder
Die HTML-Dateien referenzieren Platzhalterpfade (`img/hero.jpg`, `img/work-01.jpg` usw.).
Eigene Bilder unter denselben Dateinamen in `img/` ablegen, oder Pfade in den
HTML-Dateien anpassen.

## Lokal ansehen
`index.html` einfach im Browser öffnen — keine Build-Tools nötig.

## Ins bestehende Repo hochladen (kreativspaces/kreativstep)

```bash
git clone https://github.com/kreativspaces/kreativstep.git
cd kreativstep
# Dateien aus diesem Ordner hierher kopieren (bestehende Inhalte ggf. sichern)
git add .
git commit -m "Redesign: femininer, reduzierter Look mit Rosé-Palette"
git push origin main
```
