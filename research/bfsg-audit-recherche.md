# BFSG-Check / Barrierefreiheits-Audit – Recherche-Zusammenfassung

_Stand: 2026-02-25_

## Produktidee

**Was:** Automatisierter BFSG-Check / Barrierefreiheits-Audit als kostenpflichtiges Einstiegsprodukt – analog zum SEO-Audit auf /seo.
**Wo:** Auf `/rundum-sicher` als Haupt-CTA mit separater Checkout-Seite (analog zu `/seo/audit-buchen`).

## Rechtlicher Rahmen

### Konformitätsvermutung (kein Garantieprinzip)

- **Es gibt keine echte rechtliche Garantie** für BFSG-Konformität – das ist gewollt.
- Das Gesetz ist bewusst technologieneutral formuliert, damit es nicht an einem Standard festklebt.
- **Konformitätsvermutung durch EN 301 549 / WCAG 2.1 AA** ist das Stärkste, was man bekommen kann:
  - Solange niemand das Gegenteil nachweist, gilt die Website als gesetzeskonform.
  - Beweislast liegt beim Beschwerdeführer / der Marktüberwachungsbehörde.
- Gängiges Prinzip im deutschen und europäischen Produktrecht (analog zu CE-Kennzeichnungen).
- **In der Praxis:** Kaum jemand kann erfolgreich vorgehen, wenn WCAG 2.1 AA nachweislich erfüllt und sauber dokumentiert ist.

### Was in der Praxis üblich ist

1. **BITV-/WCAG-Audit** durch anerkannte Prüfstelle (z.B. BIK-BITV-Test) → dokumentierte Konformitätserklärung
2. **Barrierefreiheitserklärung** auf der Website veröffentlichen mit Feedback-Mechanismus
3. **Echte Nutzertests** mit betroffenen Personen (automatisierte Tools decken nur ~30-40% der Barrieren ab)

## Automatisierter Test: Möglichkeiten und Grenzen

### Was automatisiert prüfbar ist

- Von den ~86 WCAG 2.2 AA Erfolgskriterien sind nur **~30-40% zuverlässig automatisiert prüfbar**
- Automatisierung erkennt: fehlende alt-Attribute, Kontrastprobleme, fehlende Labels, ARIA-Fehler, Strukturfehler
- Automatisierung erkennt NICHT: ob Alt-Texte sinnvoll sind, ob Fokus-Reihenfolge logisch ist, ob Fehlermeldungen verständlich sind, ob Seitenstruktur semantisch korrekt ist

### Ist es rechtens, das anzubieten?

- **Ja**, keine rechtliche Hürde. Diverse Anbieter machen das (Siteimprove, WAVE, Deque/axe).
- **ABER:** Man darf nicht behaupten, dass Bestehen des Tests eine rechtsverbindliche Konformität garantiert (wäre irreführend im Sinne des Wettbewerbsrechts).
- **Kommunikation muss klar sein:** "Automatisierter Erst-Check, der X von Y maschinell prüfbaren Kriterien abdeckt. Ersetzt keine vollständige Barrierefreiheitsprüfung."

### Ist es ausreichend für Kunden?

- **Allein: Nein.** 60-70% der Barrieren werden nicht erkannt.
- **Als Einstieg: Ja** – wenn klar als erster Überblick positioniert, mit Empfehlung für weiterführende Maßnahmen.

## Technische Umsetzung

### MCP-Server / KI-Tools

| Tool | Typ | Beschreibung |
|------|-----|-------------|
| **A11y MCP** | MCP-Server, Open Source | axe-core + Puppeteer, prüft WCAG 2.0/2.1/2.2. Direkt in Claude Desktop/Cursor einbindbar |
| **BrowserStack MCP** | MCP-Server, kostenpflichtig | Accessibility-Scans aus Coding-Assistenten heraus |
| **TestSprite** | MCP-Agent | Vollautomatisiert: Keyboard-Navigation, Focus-Order, ARIA, Kontraste |
| **AccessiMind** | VS Code Extension | KI-gestützt, Echtzeit-WCAG-2.2-Analyse und ARIA-Validierung im Quellcode |
| **Deque axe DevTools** | Browser Extension | 2025: KI-Features (Auto-Remediation, Priorisierung nach Impact) |

### Open-Source-Tooling (Basis)

- **axe-core** – De-facto-Standard für automatisiertes A11y-Testing
- **pa11y** – CLI-Tool, WCAG-Prüfung
- **Lighthouse API** – Google, inkl. Accessibility-Score

### Empfohlener Ansatz

Automatisierten Test als Basis (axe-core / A11y MCP), KI-gestützte Aufbereitung der Ergebnisse mit konkreten Fix-Vorschlägen als Mehrwert gegenüber nacktem Report.

## Produktpositionierung (Entwurf)

### Passt zu /rundum-sicher weil:

- `/rundum-sicher` bündelt bereits Barrierefreiheit (BFSG, WCAG) als Thema
- Analogie zum SEO-Audit: "Ohne Analyse keine sinnvolle Empfehlung"
- Stärkt die Conversion-Strategie der Seite (aktuell nur Kontakt/Termin als CTA)
- Schafft niedrigschwelligen Einstieg ins Thema Barrierefreiheit

### Differenzierung von Wettbewerbern

- Wettbewerber ignorieren Barrierefreiheit oder setzen Overlay-Widgets ein (siehe Competitive Landscape)
- Kein Wettbewerber in Regensburg bietet einen BFSG-Check als Produkt an
- Ehrliche Kommunikation ("automatisierter Erst-Check, kein vollständiges Audit") = Vertrauen

### Offene Fragen für nächste Schritte

- [ ] **Produktumfang:** Was genau liefern wir? (Report-Format, Anzahl Seiten, Fix-Vorschläge, Besprechung?)
- [ ] **Preisfindung:** Welcher Preisbereich? (Vergleich: SEO-Audit 790-1.290€. BFSG-Check vermutlich günstiger weil automatisiert?)
- [ ] **Paketstruktur:** Analog zu SEO-Audit (Starter/Business/Commerce) oder anders?
- [ ] **Upsell-Pfad:** Check → manuelles Audit → Umsetzung der Fixes → laufende Überwachung?
- [ ] **Checkout-Seite:** `/rundum-sicher/bfsg-check-buchen` analog zu `/seo/audit-buchen`?
- [ ] **Sitemap-Erweiterung:** Neuer Eintrag unter /rundum-sicher
- [ ] **Technische Umsetzung:** A11y MCP + axe-core als Basis, KI-Aufbereitung
- [ ] **Kommunikation auf der Seite:** Klare Abgrenzung "automatisierter Erst-Check" vs. "vollständiges Audit"
