# kreativstep

Static portfolio website for **kreativstep.de** — plain HTML/CSS, no build step, no framework.

## Project structure

```
index.html   Page content
style.css    Styling
CNAME        Custom domain for GitHub Pages (kreativstep.de)
```

## Running locally

No build tools required. From the project root, start any static file server, for example:

```bash
python3 -m http.server 8080
```

Then open [http://localhost:8080](http://localhost:8080) in your browser.

Alternatives: `npx serve .`, or the VS Code "Live Server" extension for auto-reload on save.

## Deployment

The site is hosted on **GitHub Pages** and served under the custom domain `kreativstep.de` (domain registered at Wix, DNS records point to GitHub Pages).

1. GitHub repo → **Settings → Pages** → Source: `main` branch, `/ (root)`.
2. Custom domain: `kreativstep.de` (picked up from the `CNAME` file).
3. At Wix, DNS records for `kreativstep.de` point to GitHub Pages' IPs (A records) and `www` → `kreativspaces.github.io` (CNAME).
4. Once the DNS check passes, enable **Enforce HTTPS** in the Pages settings.

---

# kreativstep (Deutsch)

Statische Portfolio-Website für **kreativstep.de** — reines HTML/CSS, kein Build-Prozess, kein Framework.

## Projektstruktur

```
index.html   Seiteninhalt
style.css    Styling
CNAME        Eigene Domain für GitHub Pages (kreativstep.de)
```

## Lokal testen

Es werden keine Build-Tools benötigt. Im Projektverzeichnis einen beliebigen statischen Webserver starten, zum Beispiel:

```bash
python3 -m http.server 8080
```

Anschließend [http://localhost:8080](http://localhost:8080) im Browser öffnen.

Alternativen: `npx serve .`, oder die VS-Code-Erweiterung "Live Server" für automatisches Neuladen beim Speichern.

## Deployment

Die Website wird über **GitHub Pages** gehostet und unter der eigenen Domain `kreativstep.de` bereitgestellt (Domain registriert bei Wix, DNS-Einträge zeigen auf GitHub Pages).

1. GitHub-Repo → **Settings → Pages** → Source: Branch `main`, `/ (root)`.
2. Custom domain: `kreativstep.de` (wird aus der Datei `CNAME` übernommen).
3. Bei Wix zeigen die DNS-Einträge für `kreativstep.de` auf die IPs von GitHub Pages (A-Records), sowie `www` → `kreativspaces.github.io` (CNAME).
4. Sobald die DNS-Prüfung erfolgreich ist, **Enforce HTTPS** in den Pages-Einstellungen aktivieren.
