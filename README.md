# DER HÄUPTLING – Relaunch Inhalte

Planung, Erstellung und Optimierung aller Inhalte für den Relaunch von [derhaeuptling.de](https://derhaeuptling.de).

## Setup für Kollegen

Einmalig die benötigten Plugin-Marketplaces hinzufügen:

```bash
claude /plugin marketplace add coreyhaines31/marketingskills
claude /plugin marketplace add anthropics/skills
claude /plugin marketplace add anthropics/claude-plugins-official
```

## Struktur

- `research/` – Keyword-Recherche, Wettbewerber-Analysen
- `seiten/` – Seitenstruktur (sitemap.md) + Inhalte pro Seite (Unterordner je Seite)
- `tracking/` – Entscheidungslog, Fortschritt
- `.claude/product-marketing-context.md` – Positionierung, Zielgruppe, Brand Voice

## Status

Siehe [TODO.md](TODO.md)

## Claude Code Skills

Alle Marketing-Skills stammen aus [`coreyhaines31/marketingskills`](https://github.com/coreyhaines31/marketingskills).

| Skill (Qualified Name)                                    | Zweck                                                       |
| --------------------------------------------------------- | ----------------------------------------------------------- |
| `coreyhaines31/marketingskills:product-marketing-context` | Positionierung, Zielgruppe, Brand Voice dokumentieren       |
| `coreyhaines31/marketingskills:copywriting`               | Seitentexte schreiben (Homepage, Landing Pages, etc.)       |
| `coreyhaines31/marketingskills:copy-editing`              | Bestehende Texte überarbeiten und verbessern                |
| `coreyhaines31/marketingskills:content-strategy`          | Content-Strategie planen, Themen definieren                 |
| `coreyhaines31/marketingskills:seo-audit`                 | SEO-Probleme analysieren und diagnostizieren                |
| `coreyhaines31/marketingskills:programmatic-seo`          | SEO-Seiten skaliert mit Templates erstellen                 |
| `coreyhaines31/marketingskills:schema-markup`             | Structured Data / JSON-LD hinzufügen                        |
| `coreyhaines31/marketingskills:page-cro`                  | Conversion-Optimierung für Marketing-Seiten                 |
| `coreyhaines31/marketingskills:signup-flow-cro`           | Signup- und Registrierungsflows optimieren                  |
| `coreyhaines31/marketingskills:onboarding-cro`            | Post-Signup Onboarding und Aktivierung                      |
| `coreyhaines31/marketingskills:form-cro`                  | Formulare optimieren (Lead, Kontakt, etc.)                  |
| `coreyhaines31/marketingskills:popup-cro`                 | Popups, Modals, Overlays optimieren                         |
| `coreyhaines31/marketingskills:paywall-upgrade-cro`       | In-App Paywalls und Upgrade-Screens                         |
| `coreyhaines31/marketingskills:marketing-psychology`      | Psychologische Prinzipien für Marketing (70+ Mental Models) |
| `coreyhaines31/marketingskills:marketing-ideas`           | Marketing-Ideen und Wachstumsstrategien (139 Ansätze)       |
| `coreyhaines31/marketingskills:competitor-alternatives`   | Vergleichs- und Alternativ-Seiten erstellen                 |
| `coreyhaines31/marketingskills:email-sequence`            | E-Mail-Sequenzen und Drip-Kampagnen                         |
| `coreyhaines31/marketingskills:social-content`            | Social-Media-Inhalte erstellen und planen                   |
| `coreyhaines31/marketingskills:paid-ads`                  | Bezahlte Werbekampagnen (Google, Meta, LinkedIn)            |
| `coreyhaines31/marketingskills:launch-strategy`           | Produkt-Launches und Go-to-Market planen                    |
| `coreyhaines31/marketingskills:pricing-strategy`          | Preisgestaltung und Packaging                               |
| `coreyhaines31/marketingskills:free-tool-strategy`        | Kostenlose Tools als Marketing-Instrument                   |
| `coreyhaines31/marketingskills:referral-program`          | Empfehlungsprogramme und Viral Loops                        |
| `coreyhaines31/marketingskills:analytics-tracking`        | Analytics und Tracking einrichten (GA4, GTM)                |

Zusätzlich verfügbare Utility-Skills (nicht Marketing-spezifisch):

| Skill                                     | Quelle                     | Registriert via              |
| ----------------------------------------- | -------------------------- | ---------------------------- |
| `claude-plugins-official/frontend-design` | Claude Plugins (offiziell) | `.skills.json`               |
| `anthropics/skills/doc-coauthoring`       | Anthropic (offiziell)      | `.skills.json`               |
| `agent-browser` / `dev-browser`           | –                          | `.claude/skills/` (Symlink)  |
| `brainstorming`                           | –                          | `.claude/skills/` (Symlink)  |
| `pdf`                                     | –                          | `.claude/skills/` (Symlink)  |
| `ast-grep`                                | –                          | global (`~/.claude/skills/`) |
