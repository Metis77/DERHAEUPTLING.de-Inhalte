# Sitemap – derhaeuptling.de

## Navigation (Hauptmenü)

```
☰ Burger-Menü (immer):
  Webdesign
  SEO
  Barrierefreiheit
  Referenzen
  Über uns
  Kontakt
```

Immer Burger-Menü, auch Desktop. Leistungen direkt als Menüpunkte, kein "Leistungen"-Dropdown. Hosting und Wartung als sekundäre Links (Footer, Querverweise von Leistungsseiten).

## Seitenstruktur

```
/                              Homepage
│
├── /webdesign                 Webdesign                      🔵 Premium
│
├── /seo                       SEO (inkl. GEO & AEO)          🔵 Premium
├── /barrierefreiheit          Barrierefreiheit                🔵 Premium
│
├── /wartung-support           Wartung & Support               🟠 Bestandskunden
├── /hosting                   Hosting & Infrastruktur         🟠 Bestandskunden
│
├── /ratgeber                  Ratgeber (Hub)                  📚 Wiki
│   ├── /ratgeber/seo              SEO-Hub
│   │   ├── /ratgeber/seo/keyword-recherche
│   │   ├── /ratgeber/seo/onpage-optimierung
│   │   ├── /ratgeber/seo/technisches-seo
│   │   ├── /ratgeber/seo/local-seo
│   │   └── /ratgeber/seo/geo-aeo-einordnung
│   │
│   ├── /ratgeber/barrierefreiheit     Barrierefreiheit-Hub
│   │   ├── /ratgeber/barrierefreiheit/bfsg-anforderungen
│   │   ├── /ratgeber/barrierefreiheit/wcag-checkliste
│   │   └── /ratgeber/barrierefreiheit/aria-grundlagen
│   │
│   ├── /ratgeber/dsgvo            DSGVO-Hub
│   │   ├── /ratgeber/dsgvo/cookie-consent
│   │   ├── /ratgeber/dsgvo/datenschutzerklaerung
│   │   └── /ratgeber/dsgvo/auftragsverarbeitung
│   │
│   ├── /ratgeber/technologie      Technologie-Hub
│   │   ├── /ratgeber/technologie/sitejet-baukasten
│   │   ├── /ratgeber/technologie/contao
│   │   ├── /ratgeber/technologie/craft-cms
│   │   ├── /ratgeber/technologie/javascript-apps
│   │   ├── /ratgeber/technologie/cms-vergleich
│   │   └── /ratgeber/technologie/wordpress-alternativen
│   │
│   └── /ratgeber/webdesign        Webdesign-Hub
│       ├── /ratgeber/webdesign/website-briefing
│       ├── /ratgeber/webdesign/website-vs-webapp
│       └── /ratgeber/webdesign/was-kostet-website
│
├── /referenzen                Referenzen
│   └── /referenzen/[slug]         Case Study
│
├── /ueber-uns                 Über uns
├── /kontakt                   Kontakt
│
├── /impressum                 Impressum                       ⚫ Footer
└── /datenschutz               Datenschutz                     ⚫ Footer
```

## Legende

- 🔵 **Premium-Funnel** – Leistungsseiten → Kontakt/Termin
- 🟠 **Bestandskunden-Funnel** – Für bestehende Kunden und Infrastruktur-Interessierte → Paket buchen / Kontakt
- 📚 **Wiki/Ratgeber** – Wissensbasis, verlinkt auf Leistungsseiten und umgekehrt
- ⚫ **Footer** – Rechtliches
- ohne Markierung – Übergreifend (Referenzen, Über uns, Kontakt)

## Querverlinkung (Prinzip)

Ratgeber und Leistungsseiten verlinken immer in beide Richtungen:
- **Leistungsseite → Ratgeber:** "Mehr dazu in unserem Ratgeber: [Thema]" (für Kunden die tiefer einsteigen wollen)
- **Ratgeber → Leistungsseite:** "Wir helfen Ihnen dabei – [Leistung ansehen]" (für Kunden die Hilfe brauchen)

## Seitenaufbau pro Leistungsseite

```
1. Hero         → Claim + Subline + CTA (Termin/Kontakt)
2. Problem      → Warum braucht der Kunde das? (Customer Language)
3. Lösung       → Was genau bieten wir? (konkrete Leistungen)
4. Prozess      → Wie arbeiten wir? (4-6 Schritte, nummeriert)
5. Social Proof → 2-3 Referenzbeispiele + Testimonial
6. Technologie  → Welche Tools/CMS setzen wir ein?
7. FAQ          → 3-5 häufige Fragen (Schema.org)
8. CTA          → Kontakt/Termin-Section
```

## Webdesign – Seitenkonzept

Eine starke Seite `/webdesign` statt Unterseiten. Enthält Sections für:
- Websites (Relaunch, Neuentwicklung)
- Online-Shops (Shopify, individuelle Lösungen)
- Web-Apps (SvelteKit, React)
- UX & UI Design (als Kompetenz integriert, keine eigene Seite)

Unterseiten (`/webdesign/shops`, `/webdesign/web-apps`) nur nachrüsten wenn Keyword-Recherche relevantes eigenständiges Suchvolumen zeigt.

## Wartung & Support – Seitenkonzept

Eigenständige Leistungsseite unter `/wartung-support`. Kein Haupt-Navpunkt, aber prominent verlinkt aus:
- Footer-Navigation
- Jeder Leistungsseite ("Nach dem Launch: Wartung & Support")
- Referenzen/Case Studies

Inhalte (basierend auf bestehendem PDF-Angebot):
- Monitoring, Sicherheitsupdates, Weiterentwicklung, Support, grafische Arbeiten
- 4 Pakete: Basic (8h) / Medium (16h) / Large (32h) / Advanced (64h)
- Preisstaffelung nach Kontingent (105-120€/h)
- Hinweis auf Netzwerk/vonformat.design bei grafischen Arbeiten

## Hosting & Infrastruktur – Seitenkonzept

Eigenständige Seite `/hosting` mit Fokus auf **technische Kompetenz**, nicht auf Baukasten-Verkauf.

**Positionierung:** "Wir kümmern uns um die komplette Infrastruktur" – ein Signal an Premium-Kunden, dass die technische Basis stimmt.

**Sichtbar (Nutzen):**
- Domains & E-Mail – alles eingerichtet (Exchange, Business-Postfächer)
- Hosting & Performance – schnell, mit CDN und Monitoring
- DevOps – automatische Deployments, kein FTP
- Sicherheit – SSL, Updates, Backups
- Tracking – datenschutzkonform mit Matomo

**Für Techniker (Detail, z.B. aufklappbar):**
- Plesk, Cloudflare, Vercel, Git Actions, Deployer, Domain-Reselling, Uptime-Monitoring

**Baukasten/WordPress:** Wird NICHT aktiv auf der Website beworben. Stattdessen im persönlichen Gespräch empfohlen für Kunden ohne Budget. Verweis auf Ratgeber-Artikel `/ratgeber/technologie/sitejet-baukasten` für Self-Service-Anleitung.

## SEO-Seite – Positionierung zu GEO & AEO

GEO (Generative Engine Optimization) und AEO (Answer Engine Optimization) werden auf der `/seo`-Leistungsseite integriert – nicht als eigene Leistung, sondern als Einordnung:

- Semantik und Schema.org waren schon immer Best Practice
- GEO/AEO sind Marketing-Begriffe für Dinge die gute SEOs schon lange machen
- Ehrliche Positionierung statt Trend-Hopping → differenziert von Mitbewerbern die das als "neu" verkaufen

Im Ratgeber: `/ratgeber/seo/geo-aeo-einordnung` als ausführlicher Artikel der die Begriffe entmystifiziert.

## Ratgeber – Konzept

Öffentliches Wissenssystem mit drei Zwecken:
1. **Nachschlagewerk** für eigene Best Practices (internes Wiki)
2. **Transparenz** für Kunden ("so denken und arbeiten wir")
3. **SEO-Nebeneffekt** (rankt mit, ist aber nicht Hauptzweck)

Hub-Struktur statt Mega-Guides. Jeder Artikel 800-2.000 Wörter, fokussiert auf ein Thema.

## Entscheidungen

### Webdesign-Unterseiten → Nein, vorerst
Alles auf einer Seite mit Sections. Websites, Shops, Web-Apps und UX/UI als Bereiche, nicht als Unterseiten. Nachrüsten wenn Keyword-Recherche eigenständiges Suchvolumen zeigt.

### UX/UI-Design als eigene Leistungsseite → Nein
Kompetenz innerhalb von Webdesign, keine eigenständige Dienstleistung die Kunden separat beauftragen. Auf `/webdesign` als Section integriert.

### SEO-Unterseiten als Leistung → Nein
Eigene Ratgeber-Artikel decken Unterthemen ab. Die Leistungsseite `/seo` bleibt eine Seite.

### Hosting: Baukasten aktiv bewerben → Nein
SiteJet und WordPress werden nicht auf der Website beworben. Empfehlung im persönlichen Gespräch für Budget-Kunden. Ratgeber-Artikel als Self-Service-Anleitung.

### Städte-Landing-Pages → Nein
Regensburg-Fokus über Schema.org (`ProfessionalService`) und natürliche Erwähnung im Content.

### CMS/Technologie als Leistungsseiten → Nein
Keine `/craft-cms-agentur`-Seiten. Stattdessen ausführliche Ratgeber-Artikel zu Contao, Craft CMS etc. Die verlinken auf `/webdesign` als Leistung.

### SEA als Leistung → Nein, vorerst
Wird aktuell nicht aktiv angeboten. Kann als Ratgeber-Artikel (`/ratgeber/seo/sea-grundlagen`) vorbereitet werden. Leistungsseite nachrüsten wenn SEA ins Portfolio aufgenommen wird.
