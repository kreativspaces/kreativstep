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

The site is hosted on **GitHub Pages** (repo `kreativspaces/kreativstep`) and served under the custom domain `kreativstep.de` (domain registered at Wix, DNS records point to GitHub Pages).

GitHub side (already configured):

1. **Settings → Pages** → Source: `main` branch, `/ (root)`.
2. Custom domain: `kreativstep.de` (picked up from the `CNAME` file).

Wix side — DNS records to maintain for `kreativstep.de` (Domains → kreativstep.de → Manage DNS Records / Advanced DNS):

| Type | Host | Value |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | kreativspaces.github.io |

Optional (IPv6), AAAA records for `@`: `2606:50c0:8000::153`, `2606:50c0:8001::153`, `2606:50c0:8002::153`, `2606:50c0:8003::153`.

Remove any pre-existing Wix "parking page" A/CNAME records for the domain — otherwise it keeps resolving to Wix instead of GitHub Pages. Once the DNS check passes on GitHub, enable **Enforce HTTPS** in the Pages settings.

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

Die Website wird über **GitHub Pages** gehostet (Repo `kreativspaces/kreativstep`) und unter der eigenen Domain `kreativstep.de` bereitgestellt (Domain registriert bei Wix, DNS-Einträge zeigen auf GitHub Pages).

GitHub-Seite (bereits eingerichtet):

1. **Settings → Pages** → Source: Branch `main`, `/ (root)`.
2. Custom domain: `kreativstep.de` (wird aus der Datei `CNAME` übernommen).

Wix-Seite — zu pflegende DNS-Einträge für `kreativstep.de` (Domains → kreativstep.de → Manage DNS Records / Advanced DNS):

| Typ | Host | Wert |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | kreativspaces.github.io |

Optional (IPv6), AAAA-Records für `@`: `2606:50c0:8000::153`, `2606:50c0:8001::153`, `2606:50c0:8002::153`, `2606:50c0:8003::153`.

Vorhandene Wix-"Parkseiten"-Einträge (A/CNAME) für die Domain entfernen — sonst wird weiterhin auf Wix statt auf GitHub Pages aufgelöst. Sobald die DNS-Prüfung bei GitHub erfolgreich ist, **Enforce HTTPS** in den Pages-Einstellungen aktivieren.
