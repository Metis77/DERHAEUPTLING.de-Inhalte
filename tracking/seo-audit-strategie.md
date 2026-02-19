# SEO-Audit: Geplante Strategie derhaeuptling.de

_Erstellt mit Skill: `seo-audit`_
_Datum: 2026-02-19_
_Typ: Pre-Launch Strategie-Audit (kein Crawl, Analyse der Planungsdokumente)_

---

## Executive Summary

Die Planungsgrundlage ist solide: Klare Positionierung, durchdachte Seitenstruktur, dokumentierte Wettbewerbslandschaft, definierte Brand Voice. Für ein Projekt in dieser Phase ist das überdurchschnittlich gut vorbereitet.

**Aber: Es fehlen drei kritische Bausteine bevor Content erstellt werden sollte:**

1. **Keyword-Recherche fehlt komplett** -- die gesamte Sitemap basiert auf Intuition, nicht auf Suchdaten
2. **301-Redirect-Plan fehlt** -- ein Relaunch ohne Redirect-Mapping riskiert den bestehenden Rank-1-Status
3. **Messbare Ergebnisse fehlen** -- Case Studies ohne KPIs sind Portfolio, kein Proof

**Gesamtbewertung:** 7/10 als Planungsgrundlage. Mit den drei genannten Lücken geschlossen: 9/10.

---

## 1. Site Architecture & URL-Struktur

### Was gut ist

- **Flache Hierarchie:** Alle wichtigen Seiten maximal 2 Klicks von der Homepage entfernt
- **Saubere URLs:** Lesbar, Kleinbuchstaben, Bindestriche, Keywords wo sinnvoll (`/webdesign`, `/seo`)
- **Hub-and-Spoke für Ratgeber:** Logische Cluster-Struktur mit Hub-Seiten und Unterartikeln
- **Bewusste Entscheidung gegen Seiten-Inflation:** Keine Städte-Landingpages, keine CMS-als-Leistung-Seiten, kein Bauchladen

### Probleme

| Issue | Impact | Details |
|-------|--------|---------|
| **`/rundum-sicher` hat kein Suchvolumen** | Mittel | Branding-Begriff, den niemand googelt. Ein voller Hauptnavigations-Slot geht an eine Seite ohne organisches Traffic-Potenzial. Als Trust-Seite im Conversion-Funnel sinnvoll, aber die Keyword-Abdeckung für Barrierefreiheit, Wartung, Hosting hängt komplett an Ratgeber-Artikeln, die noch nicht existieren. |
| **URL-Inkonsistenz Datenschutz** | Niedrig | Sitemap zeigt `/ratgeber/datenschutz`, Rundum-sicher-Konzept verweist auf `/ratgeber/dsgvo/*`. Muss vor Umsetzung geklärt werden. |
| **Ratgeber-Tiefe 3 Ebenen** | Niedrig | `/ratgeber/seo/keyword-recherche` ist akzeptabel für topische Autorität, aber URLs kürzer als 3 Ebenen performen tendenziell besser. Kein Handlungsbedarf, nur Bewusstsein. |

### Empfehlung

- `/rundum-sicher` als Trust-Seite beibehalten, aber sicherstellen, dass die korrespondierenden Ratgeber-Artikel die relevanten Keywords abdecken (z.B. "barrierefreie Website erstellen lassen", "Website Wartung Kosten", "Webhosting Regensburg")
- URL-Pfad für Datenschutz-Ratgeber einheitlich festlegen

---

## 2. Keyword-Strategie & Abdeckungslücken

### Kritischer Befund: Keine Keyword-Recherche vorhanden

Die gesamte Seitenstruktur, die Ratgeber-Themen und die Content-Planung basieren auf Branchen-Intuition, nicht auf Suchdaten. Das TODO "Keyword-Recherche für geplante Landing Pages" ist noch offen.

**Warum das kritisch ist:**
- Ohne Suchvolumen-Daten ist unklar, ob die geplanten Ratgeber-Artikel überhaupt gesucht werden
- Ohne Keyword-Difficulty-Daten ist unklar, welche Keywords realistisch rankbar sind
- Ohne Search-Intent-Analyse ist unklar, ob die geplante Content-Form (Leistungsseite vs. Ratgeber) zum Intent passt

### Vermutete Keyword-Lücken (ohne Daten, basierend auf Marktkenntnis)

| Keyword-Cluster | Aktuell abgedeckt? | Potenzielles Suchvolumen |
|------------------|--------------------|--------------------------|
| "Webdesign Regensburg" | Ja, /webdesign | Hoch (aktuell Rank 1-3) |
| "Webentwicklung Regensburg" / "Webentwickler Regensburg" | Nein, keine Seite | Vermutlich mittel |
| "Homepage erstellen lassen Regensburg" | Nein | Vermutlich mittel |
| "Online Shop erstellen lassen" | Teilweise (/webdesign Section) | Vermutlich mittel |
| "Website Relaunch" | Nein, kein dedizierter Content | Vermutlich mittel |
| "SEO Regensburg" / "SEO Agentur Regensburg" | Ja, /seo | Mittel |
| "Barrierefreie Website erstellen" / "BFSG Website" | Nur über Ratgeber geplant | Vermutlich steigend (BFSG) |
| "Website Wartung" / "Website pflegen lassen" | Nur über Ratgeber geplant | Vermutlich niedrig-mittel |
| "Was kostet eine Website" | Ja, Ratgeber geplant | Hoch (informational) |

### Kannibalisierungsrisiko

- **/seo** (Leistungsseite) vs. **/ratgeber/seo/*** -- Wer rankt für "SEO Regensburg"? Die Leistungsseite muss klar transactional sein, Ratgeber klar informational. Ohne bewusste Intent-Trennung kannibalisieren sie sich.
- **/webdesign** vs. **/ratgeber/webdesign/*** -- Gleiches Risiko, gleiche Lösung.

### Empfehlung

**Keyword-Recherche VOR Content-Erstellung durchführen.** Mindestumfang:
1. Seed-Keywords identifizieren (Leistungen + Ratgeber-Themen)
2. Suchvolumen + Keyword Difficulty für Region Regensburg und national
3. Search Intent pro Keyword klassifizieren (informational / transactional / navigational)
4. Keyword-Mapping: Jede Seite bekommt EIN Primary Keyword + 2-3 Secondary Keywords
5. Content-Priorisierung anhand von Suchvolumen x Relevanz x Schwierigkeit

---

## 3. Interne Verlinkung & Topical Clustering

### Was gut ist

- Bidirektionales Verlinkungsprinzip definiert (Leistungsseite ↔ Ratgeber)
- Hub-Struktur schafft natürliche thematische Cluster

### Lücken

| Issue | Impact | Details |
|-------|--------|---------|
| **Keine Cross-Cluster-Verlinkung geplant** | Mittel | Wie verlinkt ein SEO-Ratgeber auf die Webdesign-Leistungsseite? Wie verlinkt /rundum-sicher auf Barrierefreiheits-Ratgeber? Nur Leistungsseite ↔ eigener Ratgeber ist zu eng. |
| **Referenzen nicht in Verlinkung integriert** | Mittel | Case Studies sollten auf relevante Leistungsseiten und Ratgeber verlinken. Umgekehrt sollten Leistungsseiten auf passende Case Studies verlinken. |
| **Homepage-Verlinkungsstrategie fehlt** | Hoch | Die Homepage ist die autoritärste Seite. Wie sie Link Equity auf Leistungsseiten und Ratgeber-Hubs verteilt, ist entscheidend. Kein Konzept vorhanden. |
| **Keine Anchor-Text-Strategie** | Niedrig | Interne Links sollten das Primary Keyword der Zielseite als Anchor-Text verwenden. Muss nicht jetzt geplant werden, aber bei Content-Erstellung beachten. |

### Empfehlung

Verlinkungsprinzip erweitern:
- **Leistungsseite ↔ Ratgeber** (bereits geplant)
- **Leistungsseite → Referenz** ("Beispiel: [Projekt]")
- **Ratgeber → Ratgeber** (Cross-Cluster wo thematisch sinnvoll)
- **Homepage → alle Leistungsseiten + Ratgeber-Hubs** (Link Equity verteilen)
- **Referenz → Leistungsseite** ("Mehr zu unserer [Leistung]")

---

## 4. Technisches SEO

### Was geplant ist

- Schema.org `ProfessionalService` für Local SEO
- FAQPage Schema für FAQ-Sections
- CDN (Cloudflare)
- Matomo (datenschutzkonform)

### Was fehlt

| Issue | Impact | Details |
|-------|--------|---------|
| **Kein 301-Redirect-Plan** | **Kritisch** | Dies ist ein RELAUNCH. Bestehende URLs (derhaeuptling.de) haben Rankings und Backlinks. Ohne 1:1 Redirect-Mapping von Alt nach Neu gehen alle bestehenden Rankings verloren, inkl. Rank 1-3 für "Webdesign Regensburg". |
| **Keine XML-Sitemap geplant** | Hoch | Muss automatisch generiert werden (CMS-Funktion) und bei Google Search Console eingereicht werden. |
| **Kein CMS/Framework entschieden** | Hoch | Core Web Vitals (LCP, INP, CLS) hängen massiv vom Tech-Stack ab. Ein Contao/Craft CMS performt anders als SvelteKit. Die Entscheidung beeinflusst alle technischen SEO-Maßnahmen. |
| **Schema.org unvollständig** | Mittel | Über ProfessionalService und FAQPage hinaus fehlen: `BreadcrumbList`, `Article`/`BlogPosting` für Ratgeber, `AggregateRating` für Bewertungen, `Service` für einzelne Leistungen, `HowTo` für Prozess-Sections |
| **Canonical-Strategie fehlt** | Mittel | Trailing-Slash-Konsistenz, www vs. non-www, Self-Referencing Canonicals auf jeder Seite |
| **Keine robots.txt-Planung** | Niedrig | Standard, aber sollte Sitemap-Verweis enthalten |

### Empfehlung

**Vor dem Relaunch zwingend:**
1. Alle bestehenden URLs von derhaeuptling.de crawlen/auflisten
2. 1:1 Redirect-Mapping erstellen (alt → neu)
3. CMS-Entscheidung treffen (beeinflusst Performance-Strategie)
4. XML-Sitemap automatisch generieren lassen
5. Schema.org Markup-Plan pro Seitentyp erstellen

---

## 5. Content-Qualität & E-E-A-T

### Was gut ist

- Starke Testimonial-Basis (30 Google Reviews, 5,0 Sterne, 100% 5-Sterne)
- Echte Referenzprojekte mit Wiedererkennungswert (wasserstoffatlas.de, BMW)
- Ehrliche, differenzierte Positionierung (kein Buzzword-Marketing)
- Brand Voice klar definiert und konsistent
- AEO/GEO-Positionierung ist glaubwürdig und differenzierend

### Lücken

| Issue | Impact | Details |
|-------|--------|---------|
| **Keine messbaren Ergebnisse** | **Hoch** | "Messbare Ergebnisse: Noch nicht erfasst." Case Studies ohne KPIs sind Portfolio-Seiten, kein Proof. Ucentric Media (direkter Wettbewerber) zeigt bereits messbare Rankings und Traffic-Zahlen. Das ist ein Wettbewerbsnachteil. |
| **Kein /ueber-uns-Konzept** | Hoch | E-E-A-T erfordert sichtbare Expertise. Wer ist Martin Schwenzer? Welche Erfahrung, welche Qualifikationen? Wer sind die Netzwerk-Partner? Individuelle Profile mit Kompetenzfeldern stärken E-E-A-T massiv. |
| **Keine Content-Priorisierung** | Mittel | 20+ Ratgeber-Artikel geplant, aber keine Reihenfolge. Welche Artikel unterstützen die primären Business-Ziele? Welche haben das höchste Suchvolumen? Ohne Priorisierung wird willkürlich produziert. |
| **Content-Tiefe nicht validiert** | Mittel | "800-2.000 Wörter" als Richtlinie. Aber: Was rankt aktuell für die Ziel-Keywords? Manche Themen brauchen 3.000+ Wörter, andere nur 500. Ohne Wettbewerbs-Content-Analyse ist die Vorgabe willkürlich. |
| **Keine Bild-/Visual-Strategie** | Mittel | Original-Screenshots, Diagramme, Prozess-Grafiken stärken E-E-A-T. Stockfotos schwächen. Nicht geplant. |

### Empfehlung

1. **Bestandskunden-Interviews priorisieren** (steht bereits im TODO). Mindestens 3-5 Projekte mit konkreten Vorher/Nachher-Daten
2. **/ueber-uns Konzept erstellen** -- Martin + Netzwerk-Partner mit Foto, Spezialisierung, Erfahrung
3. **Content-Priorisierung nach Keyword-Recherche** -- nicht nach Lust und Laune, sondern nach Impact

---

## 6. Conversion-Strategie & SEO-Alignment

### Was gut ist

- Klare Funnel-Stufen (Awareness → Decision)
- CTA-Strategie definiert (Kontakt/Termin)
- Vertrauenselemente geplant (Bewertungen, Logos, Testimonials)

### Lücken

| Issue | Impact | Details |
|-------|--------|---------|
| **Keine Micro-Conversions** | Mittel | Nur "Kontakt" oder "Termin" als CTA. Kein Zwischenschritt für Besucher die noch nicht bereit sind (z.B. Website-Briefing-Template als Download, SEO-Checkliste, Newsletter). Binary: Kontakt oder weg. |
| **Ratgeber-CTA unklar** | Mittel | Ratgeber-Artikel verlinken auf Leistungsseiten, aber was ist der CTA AUF dem Ratgeber? Nur ein Textlink? Ein CTA-Banner? Eine Sidebar? Das beeinflusst die Conversion-Rate des gesamten Ratgeber-Bereichs. |
| **Bewertungsquelle nicht entschieden** | Niedrig | Sitemap erwähnt ProvenExpert, Marketing-Kontext hat Google Reviews (5,0 / 30 Bewertungen). ProvenExpert ist ein externes Widget mit Cookie-Implikationen. Google Reviews sind kostenlos und vertrauenswürdiger. Entscheidung nötig. |

### Empfehlung

- Mindestens einen Lead-Magneten planen (z.B. "Website-Briefing-Vorlage" als PDF-Download gegen E-Mail)
- CTA-Konzept für Ratgeber-Artikel definieren (Empfehlung: CTA-Section am Ende + kontextuelle CTAs im Text)
- Google Reviews nativ einbinden (kein ProvenExpert-Widget nötig bei 5,0 / 30 Reviews)

---

## Priorisierter Aktionsplan

### Vor Content-Erstellung (Blocker)

| # | Aktion | Begründung |
|---|--------|------------|
| 1 | **Keyword-Recherche durchführen** | Ohne Suchdaten ist Content-Erstellung Blindflug. Betrifft ALLE Seiten. |
| 2 | **301-Redirect-Plan erstellen** | Bestehende Rankings schützen. Muss vor Relaunch stehen, aber je früher desto besser. |
| 3 | **CMS/Tech-Stack-Entscheidung** | Beeinflusst Performance, Schema-Implementation, Bild-Optimierung, alles. |

### Vor Relaunch (wichtig, aber nicht blockierend für Content)

| # | Aktion | Begründung |
|---|--------|------------|
| 4 | **/ueber-uns Konzept erstellen** | E-E-A-T-Signal, beeinflusst Vertrauenswürdigkeit aller Seiten. |
| 5 | **Bestandskunden für KPIs befragen** | Case Studies mit Zahlen sind der stärkste Differentiator vs. Wettbewerb. |
| 6 | **Schema.org Markup-Plan pro Seitentyp** | ProfessionalService, FAQPage, BreadcrumbList, Article, Service, AggregateRating. |
| 7 | **Interne Verlinkungsstrategie erweitern** | Cross-Cluster, Referenzen-Integration, Homepage-Strategie. |

### Quick Wins (parallel zur Content-Erstellung)

| # | Aktion | Begründung |
|---|--------|------------|
| 8 | **URL-Inkonsistenz klären** (/datenschutz vs. /dsgvo) | 5 Minuten, verhindert spätere Verwirrung. |
| 9 | **Bewertungsquelle entscheiden** (Google Reviews empfohlen) | Beeinflusst Design und Datenschutz-Konzept. |
| 10 | **Lead-Magnet konzipieren** | Parallel zur Content-Erstellung planbar. |

### Langfristig (nach Relaunch)

| # | Aktion | Begründung |
|---|--------|------------|
| 11 | **Content-Tiefe pro Keyword validieren** | SERP-Analyse für jedes Ziel-Keyword: Was rankt, wie lang, welches Format? |
| 12 | **Webdesign-Unterseiten evaluieren** | Nach 6 Monaten: Zeigt die Keyword-Recherche Bedarf für /webdesign/shops etc.? |
| 13 | **AI-Writing-Patterns vermeiden** | Bei Content-Erstellung: Keine Em-Dashes, keine AI-typischen Phrasen (siehe Referenz). |

---

## Fazit

Die strategische Grundlage ist stark. Positionierung, Wettbewerbsanalyse und Seitenstruktur sind überdurchschnittlich durchdacht. Die drei kritischen Lücken (Keyword-Recherche, Redirect-Plan, messbare Ergebnisse) sind alle lösbar und sollten VOR der Content-Erstellung adressiert werden.

Der größte Risikofaktor ist nicht die Planung, sondern ein zu früher Start der Content-Erstellung ohne Suchdaten-Fundament.
