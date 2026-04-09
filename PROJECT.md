# WWS Advisory GmbH – Website-Projekt

## Status
- **Stand:** 9. April 2026
- **Phase:** Landing Page fertig, GitHub deployed, noch nicht live
- **GmbH:** Noch nicht im Handelsregister eingetragen (Vorgesellschaft)

## Repository
- **GitHub:** https://github.com/wowas007/wws-advisory
- **Lokaler Pfad:** `/Users/wolfgangschmidt/wws-advisory/`
- **Einzige Datei:** `index.html` (statische Single-Page-Site)
- **GitHub Pages:** Noch nicht aktiviert – soll erst nach GmbH-Aktivierung eingeschaltet werden

## Domains
- `wws-advisory.de` und `wwsadvisory.com` sind vorhanden, noch nicht mit GitHub Pages verbunden

## Design-Entscheidungen
- **Stil:** Minimalistisch, Apple/Braun-inspiriert, links-bündig, Content unten links
- **Font:** Albert Sans (Google Fonts) – Gewichte 300/400/600
- **Farbpalette:** Fast-weiß (#fafafa), Schwarz (#1d1d1f), Grau (#86868b)
- **Layout:** Content links unten, Sprachumschalter oben rechts, Impressum/Datenschutz unten rechts (fixed)
- **Mobil:** Content zentriert, Footer wird statisch unter Content

## Typografie-Hierarchie
- **WWS** (bold 600) + **Advisory** (light 300, grau) – eine Zeile
- **GmbH · Berlin** – darunter, klein, uppercase-ish, grau
- Drei Taglines mit vertikaler Linie links
- **Wolfgang Schmidt** (600) + **Bundesminister a.D.** (300, grau)
- Link zu wolfgang-schmidt.eu mit ↗-Pfeil-Icon
- Social Icons: X, Instagram, LinkedIn (SVG)

## Sprachumschalter (DE / EN / ES)
Funktional per JavaScript, wechselt mit Fade-Animation:

| Element | DE | EN | ES |
|---|---|---|---|
| Taglines | Deutsche, europäische und internationale Politik. / Sicherheit, Technologie und Verteidigung. / Wirtschaft und Finanzen. | German, European and international politics. / Security, technology and defence. / Economy and finance. | Política alemana, europea e internacional. / Seguridad, tecnología y defensa. / Economía y finanzas. |
| Titel | Bundesminister a.D. | Former Federal Minister | Ex Ministro Federal |
| Footer links | Impressum / Datenschutz | Legal Notice / Privacy Policy | Aviso legal / Privacidad |

## Externe Links
- **Website:** https://wolfgang-schmidt.eu
- **X:** https://x.com/schmidtWS_
- **Instagram:** https://www.instagram.com/wolfgangschmidt/
- **LinkedIn:** https://www.linkedin.com/in/wolfgangschmidthamburg/
- **Impressum:** https://wolfgang-schmidt.eu/impressum.html
- **Datenschutz:** https://wolfgang-schmidt.eu/datenschutz.html

## Nächste Schritte
1. GmbH-Eintragung abwarten
2. GitHub Pages aktivieren (`gh pages` oder Settings → Pages → main branch)
3. Custom Domain verbinden (wws-advisory.de oder wwsadvisory.com)
4. DNS CNAME auf `wowas007.github.io` setzen
5. Ggf. eigenes Impressum/Datenschutz für die GmbH erstellen (statt Verweis auf Hauptseite)
6. Ggf. `<meta>` SEO-Tags, Open Graph, Favicon ergänzen

## Technische Hinweise
- Reine statische HTML-Seite, kein Build-Prozess, kein Framework
- Google Fonts wird extern geladen (Albert Sans)
- Alle Social-Icons sind inline SVG (kein externer Icon-Service)
- Sprachumschaltung rein clientseitig (kein serverseitiges Routing)
