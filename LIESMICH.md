# RFS Website Entwurf v1 (Oktober 2026)

Statische Website, Deutsch (/) und Englisch (/en/), ohne Framework. Saubere URLs ohne .html.

## Struktur
- index.html, en/index.html: Startseiten DE und EN
- impressum/, datenschutz/: Platzhalter, Texte von RFS oder Rechtsberatung einsetzen
- assets/: CSS, Schriften (Barlow, selbst gehostet, keine Google Fonts), Logo, Karte, Visual
- robots.txt (inkl. KI Crawler erlaubt), sitemap.xml mit hreflang, llms.txt (Kurzprofil für KI Suche)

## SEO
- Title, Description, Canonical, hreflang DE/EN/x-default, Open Graph, Geo Meta (Viersen)
- Eine H1 je Seite, Keywords: 3PL, Fulfillment, Viersen, Niederrhein, NRW, B2B, B2C, Container
- Bilder mit Alt Text, Lazy Loading unterhalb des ersten Bildschirms, Schriften mit font-display swap

## GEO (Sichtbarkeit in KI Antworten)
- JSON-LD: Organization + LocalBusiness (Adresse, Koordinaten, Einzugsgebiet, Mutter HEYDAY AG), WebSite, WebPage, FAQPage
- Abschnitt "RFS in einem Satz" als zitierfähige Faktenaussage
- FAQ mit acht direkten Fragen und Antworten, identisch im JSON-LD
- llms.txt mit Kerndaten, Leistungen, Systemen und Ausschlüssen

## Vor Livegang klären
- Domain bestätigen (Entwurf nutzt www.rfs-logistik.de)
- Adresse, Telefon und Mail bestätigen ([Telefonnummer] ist Platzhalter)
- Kontaktformular: POST auf /api/kontakt braucht ein Backend oder einen Formulardienst; Spamschutz per Honeypot ist eingebaut
- Open Graph Bild assets/img/og.png (1200 x 630) fehlt noch
- Echte Fotos aus der Halle ergänzen, Referenzen und Kundennamen freigeben lassen
- Impressum und Datenschutz einsetzen, Google Unternehmensprofil anlegen und mit der Seite verknüpfen
