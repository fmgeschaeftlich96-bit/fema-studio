# FeMa Studio – Portfolio

Statische Website für Felix Mauk / FeMa Studio (fema-studio.de).
Webdesign für lokale Unternehmen in Neuruppin & Umgebung.

## Tech Stack

- Reines HTML/CSS/JavaScript – kein Framework, kein Build-Tool, kein npm
- Hosting: Vercel (statisch)
- Fonts: Bunny Fonts (DSGVO-konform, kein Google Fonts)
- Analytics: Cloudflare Web Analytics

## Dateien

| Datei | Zweck |
|---|---|
| `index.html` | Hauptseite – alle Sektionen (Hero, Leistungen, Ablauf, Preise, Beispiel, FAQ, Kontakt) |
| `impressum.html` | Pflichtseite |
| `datenschutz.html` | Pflichtseite |
| `agb.html` | Allgemeine Geschäftsbedingungen |
| `404.html` | Fehlerseite |
| `vercel.json` | Redirects, Caching-Header, cleanUrls |
| `robots.txt` | Crawler-Freigabe + Sitemap-Verweis |
| `sitemap.xml` | Alle öffentlichen Seiten |
| `favicon.svg` | Primäres Favicon (modern) |
| `favicon.ico` | Fallback-Favicon (ältere Browser) |
| `apple-touch-icon.png` | iOS Home Screen Icon (180×180px) |
| `hero-bg.jpg` | Hero-Hintergrundbild |
| `felix.jpg` | Profilbild Kontaktsektion |
| `mirash-preview.jpg` | Beispiel-Screenshot (Mirash Barbershop) |
| `og-image.jpg` | Open Graph / WhatsApp Share-Bild (1200×630px) |

## Design-System

Farben (CSS Custom Properties):
- `--bg: #05050f` — Hintergrund
- `--text: #f1f5f9` — Haupttext
- `--muted: #64748b` — Gedämpfter Text
- `--muted-light: #94a3b8` — Heller gedämpfter Text
- `--indigo: #6366f1` — Akzentfarbe
- `--border: rgba(255,255,255,0.07)` — Rahmenfarbe

Fonts: Archivo (Überschriften), Space Grotesk (Fließtext)

Gradient-Akzent: `linear-gradient(135deg, #6366f1, #a855f7, #06b6d4)`

## Regeln

**Kein Redesign ohne ausdrückliche Zustimmung.**
Designänderungen (Farben, Schriften, Layout) nur wenn Felix explizit danach fragt.

**Kein auto-Deploy ohne Bestätigung.**
Nach Änderungen immer fragen: "Soll ich jetzt deployen?"

**Deployment-Workflow** (immer in dieser Reihenfolge):
```
git add <dateien> && git commit -m "..." && git push
PATH=/Users/fema/node/bin:$PATH npx vercel@latest deploy --prod
PATH=/Users/fema/node/bin:$PATH npx vercel@latest alias set <deployment-url> fema-studio.de
```

**Mirash Barbershop** – Referenz-Card ist aktuell ausgeblendet (HTML-Kommentar).
Grund: Erlaubnis des Inhabers noch ausstehend. Nicht löschen, nur auskommentiert lassen.
Wenn Erlaubnis vorliegt: Kommentar entfernen und mirash-preview.jpg reaktivieren.

**Steuernummer** fehlt noch im Impressum – wird nach Gewerbeanmeldung ergänzt.

**Rechtliches** – AGB gelten ausschließlich B2B (keine Verbraucher).
Kein Widerrufsrecht notwendig. Rechtswahl: deutsches Recht (§13 AGB).
