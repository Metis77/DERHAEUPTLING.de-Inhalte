# Sitemap – derhaeuptling.de

## Navigation (Hauptmenü)

```
☰ Burger-Menü (immer):
  Webdesign
  SEO
  Rundum sicher
  Referenzen
  Über uns
  Kontakt
```

Immer Burger-Menü, auch Desktop. Grund: Viele Menüpunkte lassen sich schwer in einer Zeile sauber positionieren – Burger hält die Seite clean und lenkt den Fokus auf den Content. Leistungen direkt als Menüpunkte, kein "Leistungen"-Dropdown.

## Seitenstruktur

```
/                              Homepage
│
├── /webdesign                 Webdesign                      🔵 Premium
│
├── /seo                       SEO (inkl. GEO & AEO)          🔵 Premium
│
├── /rundum-sicher            Rundum sicher                   🔵 Premium
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
│   ├── /ratgeber/datenschutz          Datenschutz (praxisnah)
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
└── /datenschutzerklaerung     Datenschutzerklärung            ⚫ Footer
```

## Legende

- 🔵 **Premium-Funnel** – Leistungsseiten → Kontakt/Termin
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

## Homepage – Seitenkonzept

TODO: Konzept erstellen. Die Homepage ist die meistbesuchte Seite und der erste Eindruck – braucht ein eigenes Konzept (Hero, Leistungsübersicht, Social Proof, CTA-Strategie).

## Referenzen – Seitenkonzept

TODO: Konzept erstellen. Aufbau für `/referenzen` (Übersichtsseite) und `/referenzen/[slug]` (einzelne Case Study). Angelehnt an: Problem → Lösung → Ergebnis. Template analog zum Seitenaufbau für Leistungsseiten definieren.

## Webdesign – Seitenkonzept

Eine starke Seite `/webdesign` statt Unterseiten. Enthält Sections für:

- Websites (Relaunch, Neuentwicklung)
- Online-Shops (Shopify, individuelle Lösungen)
- Web-Apps (SvelteKit, React)
- UX & UI Design (als Kompetenz integriert, keine eigene Seite)

Unterseiten (`/webdesign/shops`, `/webdesign/web-apps`) nur nachrüsten wenn Keyword-Recherche relevantes eigenständiges Suchvolumen zeigt.

## Rundum sicher – Seitenkonzept

Konsolidierte Seite `/rundum-sicher`. Bündelt Barrierefreiheit, Datenschutz, Rechtssicherheit, Wartung, Hosting und Monitoring auf einer Seite. Haupt-Navpunkt.

**Positionierung:** Sicherheitsversprechen für Neukunden (Pre-Sales). Adressiert das Bedürfnis: "Ich will sicher sein, dass an alles gedacht wurde – bei der Erstellung und danach." Keine Keyword-Seite, sondern Trust-/Conversion-Seite.

**Seitenaufbau:**

1. Hero → "Rundum sicher" + Subline + CTA
   Subline-Richtung: "Von der ersten Zeile Code bis zum laufenden Betrieb – wir denken an alles."
2. Problem → Was passiert wenn niemand mitdenkt?
   (Rechtsmängel, Datenschutzlücken, Ausfälle, veraltete Software, unzugängliche Seiten)
3. Bei der Erstellung → Was wir von Anfang an richtig machen:
   - Barrierefreiheit (BFSG, WCAG – kein Overlay)
   - Datenschutz & Integrationen (Privacy-by-Design: Tools wählen die keinen Consent brauchen. Consent Manager richtig einrichten wenn doch nötig.)
   - Rechtssicherheit (Impressum, DSGVO-Konformität)
     Jeweils aufklappbar → technische Details
4. Nach dem Launch → Was wir dauerhaft im Blick behalten:
   - Wartung & Updates
   - Hosting & Performance
   - Sicherheit & Backups
   - Monitoring & Reporting
   - Weiterentwicklung
     Jeweils aufklappbar → technische Details
5. So arbeiten wir → Fester Ansprechpartner, Reaktionszeiten, Stundenkontingente
6. Social Proof → Testimonial zur Betreuung + "Seit X Jahren betreut"-Zahlen
7. FAQ → Schema.org FAQPage
8. CTA → Kontakt

**Technische Details (aufklappbar):**

- Webhosting auf eigenen Servern mit Plesk-Verwaltung
- Domains über externen Domain-Reseller
- E-Mail: Microsoft Exchange und Business-Postfächer
- CDN: Cloudflare
- DevOps: Git Actions, Deployer, Vercel (für JS-Apps)
- Uptime-Monitoring
- Tracking: Matomo (datenschutzkonform)

**Wartungspakete (Referenz aus bestehendem PDF-Angebot):**

- 4 Pakete: Basic (8h) / Medium (16h) / Large (32h) / Advanced (64h)
- Preisstaffelung nach Kontingent (105-120€/h)
- Hinweis auf Netzwerk/vonformat.design bei grafischen Arbeiten

**Baukasten/WordPress:** Wird NICHT aktiv auf der Website beworben. Stattdessen im persönlichen Gespräch empfohlen für Kunden ohne Budget. Verweis auf Ratgeber-Artikel `/ratgeber/technologie/sitejet-baukasten` für Self-Service-Anleitung.

**Tiefe in Ratgeber auslagern:**

- `/ratgeber/barrierefreiheit/*` – BFSG, WCAG, ARIA
- `/ratgeber/dsgvo/*` – Cookie Consent, Datenschutzerklärung, AVV
- Ggf. `/ratgeber/webdesign/website-wartung-kosten`

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

### Barrierefreiheit, Wartung, Hosting als Einzelseiten → Nein

Konsolidiert zu `/rundum-sicher`. Alle drei Themen adressieren dasselbe Kundenbedürfnis: Sicherheit. "Bei der Erstellung" (Barrierefreiheit, Datenschutz, Recht) und "Nach dem Launch" (Wartung, Hosting, Monitoring) als zwei Phasen auf einer Seite. Tiefe über Ratgeber-Artikel.

### Hosting: Baukasten aktiv bewerben → Nein

SiteJet und WordPress werden nicht auf der Website beworben. Empfehlung im persönlichen Gespräch für Budget-Kunden. Ratgeber-Artikel als Self-Service-Anleitung.

### Städte-Landing-Pages → Nein

Regensburg-Fokus über Schema.org (`ProfessionalService`) und natürliche Erwähnung im Content.

### CMS/Technologie als Leistungsseiten → Nein

Keine `/craft-cms-agentur`-Seiten. Stattdessen ausführliche Ratgeber-Artikel zu Contao, Craft CMS etc. Die verlinken auf `/webdesign` als Leistung.

### DSGVO als eigener Hub mit 3 Artikeln → Nein

Stattdessen ein praxisnaher Datenschutz-Artikel der zeigt, wie Website-Datenschutz pragmatisch umgesetzt wird (Consent, Datenschutzerklärung, AV-Verträge). Positionierung: Gegen unnötige und falsch konfigurierte Consent-Manager-Automatismen – für pragmatischen, korrekten Datenschutz. Keyword-Relevanz in der Recherche prüfen.

### SEA als Leistung → Nein, vorerst

Wird aktuell nicht aktiv angeboten. Kann als Ratgeber-Artikel (`/ratgeber/seo/sea-grundlagen`) vorbereitet werden. Leistungsseite nachrüsten wenn SEA ins Portfolio aufgenommen wird.

## Conversion-Strategie

### Funnel-Stufen

1. **Awareness:** SEO-Landing-Pages ranken für Ziel-Keywords
2. **Interest:** Leistung + Prozess + Referenzbeispiele zeigen
3. **Consideration:** Social Proof (Bewertungen, Logos, Referenzen)
4. **Decision:** CTA je nach Seitentyp (Kontakt/Termin)

### Vertrauenselemente (auf allen Leistungsseiten)

- Kundenbewertungen prominent einbinden (z.B. ProvenExpert, Google Reviews)
- Kundenlogos zeigen wo möglich
- Transparenzversprechen / Arbeitsweise offenlegen
- **Testimonials mit Namen + Rolle** (z.B. "Geschäftsführer, Firma X")
- **Case Studies statt nur Portfolio:** Problem → Lösung → Ergebnis erzählen

### Technisches SEO

- Schema.org Structured Data (`ProfessionalService`) für lokales SEO in Regensburg
- Jede Leistungsseite mit eigenem Schema-Markup

## Inspirationsquellen

| Seite               | Was sie gut machen                                                                                                              | Relevant für uns                                     |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------- |
| lau.do              | SEO-Landing-Pages pro Leistung, Prozess-Visualisierung, ProvenExpert-Bewertungen, starkes Portfolio                             | Landing-Page-Struktur, Prozess sichtbar machen       |
| webdesign-berlin.de | Lead-Gen-Fokus, Transparenzversprechen, Video-Einbindung                                                                        | Vertrauenselemente, aktive Lead-Generierung          |
| bigdropinc.com      | Testimonials mit Name+Titel, Case Studies (Problem→Lösung→Ergebnis), Schema.org Structured Data, AI-Services als Zukunftssignal | Case-Study-Format, Testimonial-Strategie, Schema.org |
