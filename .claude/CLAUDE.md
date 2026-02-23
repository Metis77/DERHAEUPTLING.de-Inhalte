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

1. **Simplicity over cleverness** - Inhalte sofort verständlich schreiben
2. **Bestehende Muster nutzen** - Etablierte Content-Patterns verwenden, nichts neu erfinden
3. **Bestehende Konventionen einhalten oder bessere vorschlagen**

## Projektstruktur

```
DH Inhalte/
├── research/              # Keyword-Recherche, Wettbewerber-Analysen
├── seiten/                # Seitenstruktur + Inhalte pro Seite
│   ├── sitemap.md         # Informationsarchitektur & Seitenkonzepte
│   └── webdesign/         # (Unterordner je Seite)
├── tracking/              # Entscheidungslog, Fortschritt
└── .claude/
    └── product-marketing-context.md  # WER/WAS/FÜR WEN
```

## Wichtige Kontextdokumente

- **TODO.md** (Root) – Aufgaben und Fortschritt. Bei Sessionstart lesen, nach erledigten Aufgaben aktualisieren.
- **Product Marketing Context:** `.claude/product-marketing-context.md` – Positionierung, Zielgruppe, Differenzierung, Brand Voice. Erstellt mit Skill `product-marketing-context`.
- **Sitemap:** `seiten/sitemap.md` – WIE die Website gebaut ist (Struktur, Seitenkonzepte, Technik, Conversion-Strategie).

## Häufige Fehler – nicht wiederholen

- Kunden nicht dumm dastehen lassen (z.B. Baukasten-Nutzer)
- Bei Dokumenten die mit einem Skill erstellt wurden: Skill-Namen oben notieren
