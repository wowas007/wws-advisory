# wws-advisory.de — Redirect-Repository

**Domain:** [wws-advisory.de](https://wws-advisory.de/)
**Verhalten:** Leitet seit 2026-04-29 auf `https://wwsadvisory.com/?lang=de` weiter.

## Architektur-Hintergrund
Bis 2026-04-29 war dies das produktive Repo für eine eigenständige WWS-Advisory-Landing. Mit Live-Gang von wwsadvisory.com als Hauptdomain (EN-Default) wurde wws-advisory.de zur Redirect-Domain — analog zur symmetrischen Struktur:

- **Privatsphäre:** wolfgang-schmidt.eu ← office-ws.de leitet weiter
- **GmbH:** wwsadvisory.com ← wws-advisory.de leitet weiter

## Inhalt
- `index.html` — meta-refresh + JS-Redirect auf `https://wwsadvisory.com/?lang=de` (Hash und Path werden mitgenommen)
- `CNAME` — `wws-advisory.de`
- `alternative-dark.html` — archivierte dunkle Designvariante der ehemaligen Landing (nicht produktiv)
- `fonts/`, `legal.css`, `impressum*.html`, `datenschutz*.html` — Reste der ehemaligen Landing, derzeit ohne Verlinkung von index.html aus erreichbar (über Direkteingabe). Kann beim nächsten Aufräumen entfernt werden, wenn der Redirect stabil läuft.

## GitHub Pages
- Repo: `wowas007/wws-advisory`
- Custom Domain: wws-advisory.de
- HTTPS: enforced
- Domain wurde am 2026-04-29 vom Repo `wws-advisory-de` (jetzt verwaist) hierhin umgehängt

## Wenn der Redirect angepasst werden muss
Im `index.html` die `meta http-equiv="refresh"`-URL und den `window.location.replace`-Aufruf gleichzeitig anpassen (beide müssen synchron sein, damit Browser ohne JS und mit JS dasselbe Verhalten zeigen).
