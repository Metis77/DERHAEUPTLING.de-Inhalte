# Claude Code Projektregeln

## Project Overview

- **Name**: Inhalte / Architektur / Planung
- **Purpose**: SEO und Conversionoptimierte Inhalte / Strukturen planen / erstellen für den Relaunch von derhaeuptling.de

## Workflow Patterns

**Neue Inhalte / Seiten**

1. Recherche → Struktur planen → Entwurf → Review

**Bestehende Inhalte optimieren**

1. Ist-Zustand analysieren → Schwächen identifizieren → Optimierung vorschlagen → Review

## Core Principles

1. **Simplicity over cleverness** - Write Content that's immediately understandable
2. **Leverage existing solutions** - Use standard Patterns, don't reinvent
3. **Early returns** - Guard clauses over nested conditionals
4. **Match existing patterns or suggest better** - Follow the projects conventions exactly or suggest better pattern

## Kritisches Hinterfragen

**WICHTIG:** Anfragen und Angaben des Nutzers sollen kritisch hinterfragt werden. Wenn eine Idee oder ein Ansatz nicht sinnvoll erscheint:

- Dagegen argumentieren und Bedenken klar äußern
- Den Vorschlag ablehnen, wenn er problematisch ist
- Alternative Lösungen aufzeigen und begründen

Ziel: Bessere Ergebnisse durch konstruktiven Widerspruch statt blindes Ausführen.

## Projektstruktur

```
DH Inhalte/
├── research/              # Keyword-Recherche, Wettbewerber-Analysen
├── sitemap/               # Seitenstruktur & Informationsarchitektur
├── seiten/                # Inhalte pro Seite
│   ├── homepage/
│   ├── webdesign/
│   ├── seo/
│   ├── barrierefreiheit/
│   ├── ux-ui/
│   ├── baukasten/
│   ├── referenzen/
│   ├── ueber-uns/
│   └── kontakt/
├── tracking/              # Entscheidungslog, Fortschritt
└── .claude/
    └── product-marketing-context.md  # Positionierung, Zielgruppe, Voice etc.
```

## Wichtige Kontextdokumente

- **TODO.md** (Root) – Aufgaben und Fortschritt. Bei Sessionstart lesen, nach erledigten Aufgaben aktualisieren.
- **Product Marketing Context:** `.claude/product-marketing-context.md` – Positionierung, Zielgruppe, Differenzierung, Brand Voice, Conversion-Strategie. Wird von Marketing-Skills automatisch referenziert.
