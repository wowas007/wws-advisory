# WWS Advisory GmbH – Website-Projekt

## Status
- **Stand:** 9. April 2026
- **Phase:** Landing Page fertig, GitHub deployed, noch nicht live
- **GmbH:** Noch nicht im Handelsregister eingetragen (Vorgesellschaft)

## Repository
- **GitHub:** https://github.com/wowas007/wws-advisory
- **Lokaler Pfad:** `/Users/wolfgangschmidt/wws-advisory/`
- **GitHub Pages:** Noch nicht aktiviert – soll erst nach GmbH-Aktivierung eingeschaltet werden

## Dateien
| Datei | Beschreibung |
|---|---|
| `index.html` | Helle Version (Hauptvariante) – #fafafa Hintergrund |
| `index-dark.html` | Dunkle Version – #1e2a3a Hintergrund (angelehnt an wolfgang-schmidt.eu), ggf. Farbwert noch anpassen |
| `PROJECT.md` | Diese Dokumentation |

## Domains
- `wws-advisory.de` und `wwsadvisory.com` sind vorhanden, noch nicht mit GitHub Pages verbunden

## Design-Entscheidungen
- **Stil:** Minimalistisch, Apple/Braun-inspiriert, links-bündig, Content unten links
- **Font:** Albert Sans (Google Fonts) – Gewichte 300/400/600
- **Helle Version:** Hintergrund #fafafa, Text #1d1d1f, Muted #86868b
- **Dunkle Version:** Hintergrund #1e2a3a, Text #e8eaed, Muted rgba(255,255,255,0.5), Akzent weiß
- **Layout:** Content links unten, Sprachumschalter (DE/EN/ES) oben rechts, Impressum/Datenschutz fixed unten rechts
- **Mobil (<600px):** Content zentriert, Footer wird statisch unter Content

## Typografie-Hierarchie
1. **WWS** (bold 600) + **Advisory** (light 300, grau) – eine Zeile
2. **GmbH · Berlin** – darunter, klein, grau
3. Drei Taglines mit vertikaler Linie links (1.5px)
4. **Wolfgang Schmidt** (600) + **Bundesminister a.D.** (300, grau)
5. ↗ wolfgang-schmidt.eu (Link mit animiertem Pfeil-Icon)
6. Social Icons: X, Instagram, LinkedIn (inline SVG, 18px)

## Sprachumschalter (DE / EN / ES)
Funktional per JavaScript, wechselt mit Fade-Animation (200ms opacity transition):

| Element | DE | EN | ES |
|---|---|---|---|
| Zeile 1 | Deutsche, europäische und internationale Politik. | German, European and international politics. | Política alemana, europea e internacional. |
| Zeile 2 | Sicherheit, Technologie und Verteidigung. | Security, technology and defence. | Seguridad, tecnología y defensa. |
| Zeile 3 | Wirtschaft und Finanzen. | Economy and finance. | Economía y finanzas. |
| Titel | Bundesminister a.D. | Former Federal Minister | Ex Ministro Federal |
| Footer 1 | Impressum | Legal Notice | Aviso legal |
| Footer 2 | Datenschutz | Privacy Policy | Privacidad |

## Externe Links (verifiziert aus Quellcode wolfgang-schmidt.eu)
- **Website:** https://wolfgang-schmidt.eu
- **X:** https://x.com/W_Schmidt_
- **Instagram:** https://www.instagram.com/wowashamburg/
- **LinkedIn:** https://www.linkedin.com/in/wolfgang-schmidt-germany
- **Impressum:** https://wolfgang-schmidt.eu/impressum.html
- **Datenschutz:** https://wolfgang-schmidt.eu/datenschutz.html

## Git-Historie
| Commit | Beschreibung |
|---|---|
| `087b227` | Initial WWS Advisory landing page |
| `267cbdf` | Add project documentation |
| `0f444e5` | Fix social links (from wolfgang-schmidt.eu), add dark variant |

## Nächste Schritte
1. GmbH-Eintragung abwarten
2. Hintergrundfarbe der dunklen Variante exakt an wolfgang-schmidt.eu anpassen (CSS-Datei der Hauptseite prüfen)
3. Entscheiden: helle oder dunkle Version als Hauptseite
4. GitHub Pages aktivieren (Settings → Pages → main branch)
5. Custom Domain verbinden (wws-advisory.de oder wwsadvisory.com)
6. DNS: CNAME auf `wowas007.github.io` setzen
7. Ggf. eigenes Impressum/Datenschutz für die GmbH erstellen (statt Verweis auf Hauptseite)
8. Ggf. `<meta>` SEO-Tags, Open Graph, Favicon ergänzen
9. Git global user config setzen: `git config --global user.email "ws@wolfgang-schmidt.eu"` + `git config --global user.name "Wolfgang Schmidt"`

## Technische Hinweise
- Reine statische HTML-Seite, kein Build-Prozess, kein Framework
- Google Fonts wird extern geladen (Albert Sans)
- Alle Social-Icons sind inline SVG (kein externer Icon-Service)
- Sprachumschaltung rein clientseitig (kein serverseitiges Routing)
- GitHub Account: `wowas007`, authentifiziert via `gh` CLI (keyring)
