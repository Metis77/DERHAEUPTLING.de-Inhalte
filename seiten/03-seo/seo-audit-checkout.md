# /seo/audit-buchen – Checkout-Seite (v1)

_Erstellt mit Skill: `copywriting`_
_Quellen: seo.md (Audit-Section, Pricing), product-marketing-context.md, sitemap.md_

**URL:** `/seo/audit-buchen`
**Seitentyp:** Checkout (kein Index, noindex)
**Einstieg:** CTA-Klick von `/seo`
**Meta Title:** SEO-Audit buchen – DER HÄUPTLING
**Robots:** noindex, follow

---

## 1. Intro

> ### SEO-Audit buchen

Sie wissen, dass Ihre Website mehr kann. Der erste Schritt: eine saubere Analyse.

Unser SEO-Audit deckt auf, was Ihre Website zurückhält – technisch, inhaltlich und strategisch. Sie erhalten einen priorisierten Maßnahmenplan und eine persönliche Ergebnis-Besprechung.

`[Link]` ← Alle Details zum SEO-Audit → /seo

**Ihr Audit umfasst:**

- ✓ Technik-Check (Crawling, Indexierung, Ladezeiten, Core Web Vitals, Schema.org)
- ✓ Onpage-Analyse (Meta-Daten, Überschriften, Bilder, interne Verlinkung)
- ✓ Keyword- & Wettbewerbsanalyse inkl. Backlink-Profil
- ✓ Content & Struktur mit E-E-A-T-Bewertung
- ✓ UX-Analyse (Navigation, Nutzerführung, Conversion-Pfade)
- ✓ Local SEO (Google Business Profile, NAP, Brancheneinträge)
- ✓ Priorisierter Maßnahmenplan
- ✓ Persönliche Ergebnis-Besprechung

### Anmerkungen

- Kurz und bestätigend. Der Besucher kommt von /seo, hat die Details bereits gelesen. Hier kein Nachverkaufen, sondern Bestätigung der Entscheidung.
- Rücklink zur /seo-Seite für Besucher die direkt auf der Checkout-Seite landen (Bookmark, weitergeleiteter Link) oder nochmal nachlesen wollen.
- Checkliste als kompakte Erinnerung: "Das bekomme ich alles dafür." Bestätigt die Kaufentscheidung ohne den Fließtext von /seo zu wiederholen. Spiegelt die 8 Bestandteile von /seo Section 4.
- noindex: Checkout-Seiten sollen nicht ranken. Follow beibehalten für interne Linkstruktur.

---

## 2. Paketauswahl

| Paket        | Für wen                                      | Preis         |
| ------------ | -------------------------------------------- | ------------- |
| **Starter**  | Unternehmenswebsite ohne Shop                | 790 € netto   |
| **Business** | Website mit Blog oder umfangreicher Struktur | 1.290 € netto |
| **Commerce** | Online-Shop oder komplexe Funktionalität     | auf Anfrage   |

`[Radio-Auswahl]` Starter / Business / Commerce

Bei **Commerce** wird im Formular der CTA angepasst:
- Preis-Anzeige entfällt (stattdessen: "Preis auf Anfrage")
- CTA-Button: "Unverbindlich anfragen" statt "Jetzt verbindlich buchen"
- Kein Kauf, sondern Anfrage – gleiche Datenfelder, aber der Hinweis ändert sich:
> Wir melden uns innerhalb von 24 Stunden mit einem individuellen Angebot.

### Anmerkungen

- Paketauswahl als Radio-Buttons, nicht als separate Seiten. Ein Klick, kein Navigieren.
- Commerce nutzt denselben Flow wie Starter/Business – nur der Abschluss ist eine Anfrage statt ein Kauf. So bleibt der Prozess konsistent und der Kunde muss nicht auf eine andere Seite wechseln.
- Gleiche Tabelle wie auf /seo – Konsistenz, kein Überraschungseffekt.

---

## 3. Kaufformular (Pre-Purchase)

> ### Ihre Daten

Nur das Nötigste – alles Weitere klären wir nach der Buchung.

**Pflichtfelder:**

| Feld              | Typ       | Hinweis                                |
| ----------------- | --------- | -------------------------------------- |
| Vorname           | Text      |                                        |
| Nachname          | Text      |                                        |
| E-Mail            | E-Mail    | Für Auftragsbestätigung                |
| Firma             | Text      |                                        |
| Straße + Nr.      | Text      | Rechnungsadresse                       |
| PLZ + Ort         | Text      |                                        |
| Website-URL       | URL       | Die Website, die auditiert werden soll |
| USt-IdNr.         | Text      | Optional, für Rechnungen               |

**Zahlung:**

`[Stripe Elements]` Eingebettetes Zahlungsfeld (Kreditkarte, SEPA-Lastschrift, PayPal, Klarna, giropay)

`[Checkbox]` Ich akzeptiere die AGB und Widerrufsbelehrung.
`[Checkbox]` Ich habe die Datenschutzerklärung gelesen.

`[CTA-Button]` Jetzt verbindlich buchen – [Preis] € netto

Unter dem Button:
Sichere Zahlung. Ihre Daten werden verschlüsselt übertragen.

### Anmerkungen

- **Eigener Checkout, Stripe im Hintergrund.** Kein Redirect zu Stripe, kein Stripe-Branding. Volle Kontrolle über UX und Daten. Umsetzung mit SvelteKit + Stripe Payment Intents + Stripe Elements (`@stripe/stripe-js`).
- **Alle Daten auf eigener Seite:** Rechnungsadresse, Kontaktdaten, Website-URL – alles in einem Formular. Stripe Elements nur für die Zahlungseingabe (Karte/SEPA). PCI-Compliance bleibt gewahrt, da Kartendaten nie den eigenen Server berühren.
- Website-URL als Pflichtfeld: Wir brauchen sie für den Audit, und der Kunde weiß sie.
- USt-IdNr. optional: Nicht jedes KMU hat eine, aber B2B-Kunden brauchen sie auf der Rechnung.
- CTA mit dynamischem Preis: "Jetzt verbindlich buchen – 790 € netto" bzw. "– 1.290 € netto". Klarheit, kein Überraschungsmoment.
- Rechtliche Checkboxen: Minimum für Fernabsatzrecht. AGB + Widerrufsbelehrung müssen vor Kaufabschluss akzeptiert werden.

---

## 4. Bestätigungsseite + Detail-Formular (Post-Purchase)

> ### Vielen Dank für Ihre Buchung!

Ihre Buchung ist eingegangen. Sie erhalten in Kürze eine Bestätigung per E-Mail.

**Damit wir direkt mit der Analyse starten können, brauchen wir noch ein paar Angaben zu Ihrem Projekt.** Das dauert nicht lange und verbessert die Qualität Ihres Audits enorm.

---

### Projekt-Details (Post-Purchase-Formular)

| Feld                         | Typ        | Pflicht | Hinweis                                             |
| ---------------------------- | ---------- | ------- | --------------------------------------------------- |
| Website-URL                  | URL        | Ja*     | *Nur wenn nicht im Kaufformular angegeben           |
| Branche / Tätigkeit          | Text       | Nein    | "In 2-3 Worten: Was macht Ihr Unternehmen?"         |
| Primäre Zielgruppe           | Text       | Nein    | "Wen wollen Sie mit Ihrer Website erreichen?"       |
| Wichtigste Ziele             | Checkboxen | Nein    | Mehr Anfragen / Mehr Sichtbarkeit / Bessere Rankings / Mehr Umsatz (Shop) / Anderes |
| Google Search Console Zugang | Radio      | Nein    | Ja, kann ich freigeben / Nein / Weiß ich nicht      |
| Google Analytics Zugang      | Radio      | Nein    | Ja, kann ich freigeben / Nein / Weiß ich nicht      |
| Bekannte Probleme            | Textarea   | Nein    | "Gibt es etwas, das Ihnen an Ihrer Website auffällt?" |
| Bisherige SEO-Maßnahmen      | Textarea   | Nein    | "Wurde schon mal SEO gemacht? Wenn ja, was?"        |
| Wunschtermin Besprechung     | Datum      | Nein    | "Wann passt Ihnen die Ergebnis-Besprechung?"        |
| Sonstiges                    | Textarea   | Nein    | "Noch etwas, das wir wissen sollten?"               |

`[CTA-Button]` Angaben absenden

Unter dem Formular:
Falls Sie gerade nicht alle Infos parat haben: Sie können das Formular auch später über den Link in Ihrer Bestätigungs-E-Mail ausfüllen.

### Anmerkungen

- **Post-Purchase = kein Kaufrisiko, aber maximale Motivation.** Der Kunde hat gerade gekauft – jetzt ist die Bereitschaft am höchsten, das Projekt voranzubringen. Diese Daten sind keine Höflichkeit, sondern bestimmen die Qualität des Audits.
- **Kein Feld ist Pflicht, aber die Kommunikation ist klar:** Wir brauchen diese Angaben. Wer sie nicht sofort hat, kann sie per E-Mail-Link nachreichen – aber das Formular wird nicht als „optional" geframt.
- Search Console / Analytics Zugang: Wichtig für den Audit, aber "Weiß ich nicht" als Option vermeidet Überforderung. Wir klären das dann im Gespräch.
- Wunschtermin: Gibt dem Kunden Kontrolle über den Zeitplan. Reduziert "Wann höre ich was?"-Unsicherheit.
- "Bisherige SEO-Maßnahmen": Hilft uns, den Audit-Fokus zu setzen und nicht Dinge zu analysieren, die der Kunde schon weiß.
- Fallback per E-Mail-Link: Für Kunden die nicht sofort alle Infos parat haben. Kein Druck, aber auch kein „ist ja egal".

---

## 5. Bestätigungs-E-Mail (Trigger: nach Kauf)

**Betreff:** Ihre SEO-Audit Buchung – nächste Schritte

> Hallo [Vorname],
>
> vielen Dank für Ihre Buchung. Hier eine kurze Zusammenfassung:
>
> **Ihr Paket:** [Starter / Business]
> **Preis:** [790 / 1.290] € netto
> **Website:** [URL, falls angegeben]
>
> **So geht es weiter:**
> 1. Ihre Rechnung erhalten Sie in Kürze per E-Mail.
> 2. Wir starten mit der Analyse Ihrer Website.
> 3. Innerhalb weniger Werktage erhalten Sie Ihren Audit-Report und wir vereinbaren die persönliche Ergebnis-Besprechung.
>
> **Nächster Schritt:** Bitte füllen Sie noch kurz die Projekt-Details aus – das hilft uns, Ihren Audit gezielt vorzubereiten: [Link zum Post-Purchase-Formular]
>
> Bei Fragen erreichen Sie mich jederzeit unter [E-Mail] oder [Telefon].
>
> Viele Grüße
> Martin Schwenzer

### Anmerkungen

- Bestätigung + nächste Schritte = Unsicherheit reduzieren. Der Kunde weiß sofort, was passiert.
- Link zum Post-Purchase-Formular als klarer nächster Schritt – nicht als Option, sondern als Erwartung. Für Kunden die es auf der Bestätigungsseite übersprungen haben.
- Persönlich von Martin, nicht von "Team DER HÄUPTLING" – konsistent mit 1-Person-SEO-Positionierung.

---

## Technische Hinweise

- **Stack:** SvelteKit + `stripe` (Node SDK, serverseitig) + `@stripe/stripe-js` (Stripe Elements, clientseitig).
- **Payment:** Stripe Payment Intents API. Eigener Checkout – kein Redirect, kein Stripe-Branding. Stripe Elements für Zahlungseingabe (PCI-compliant).
- **Flow Starter/Business:**
  1. Kunde füllt Formular aus (Kontakt + Rechnungsadresse + URL + Zahlungsmethode via Stripe Elements)
  2. SvelteKit Form Action (`+page.server.ts`) erstellt Stripe Customer + PaymentIntent serverseitig
  3. `stripe.confirmPayment()` clientseitig bestätigt Zahlung
  4. Bei Erfolg: Redirect zu Bestätigungsseite mit Post-Purchase-Formular
- **Flow Commerce:** Gleiche Felder (ohne Stripe Elements), Submit sendet Anfrage per E-Mail. Bestätigungsseite mit Hinweis auf Rückmeldung.
- **Stripe Webhooks:** `payment_intent.succeeded` → Bestätigungs-E-Mail auslösen, Buchhaltung anstoßen. Webhook als Fallback – nicht auf Client-Redirect verlassen.
- **Post-Purchase-Formular:** Auf Bestätigungsseite inline + als eigene URL für E-Mail-Link (z.B. `/seo/audit-buchen/details`).
- **E-Mail-Versand:** Transaktionale E-Mail via Postmark oder Resend (Webhook-Trigger).
- **Tracking:** Conversion-Event bei erfolgreicher Zahlung (Matomo).
- **Schema.org:** `Product` + `Offer` Markup für die Paketauswahl (auch wenn noindex).

---

## Offene Punkte

- [ ] **AGB + Widerrufsbelehrung:** Müssen erstellt werden (Fernabsatzrecht). Juristisch prüfen lassen.
- [ ] **Stripe-Rechnungen:** Stripe Invoicing nutzen oder eigene Rechnungen aus Buchhaltungssoftware (z.B. lexoffice)?
- [ ] **Stripe Tax:** Automatische USt-Berechnung über Stripe Tax oder manuell?
- [ ] **Post-Purchase-Formular URL:** Eigene Route (z.B. `/seo/audit-buchen/details`) oder nur auf Bestätigungsseite?
- [ ] **E-Mail-Tool:** Postmark, Resend, oder über Craft CMS Plugin?
- [x] **Zahlungsmethoden:** Kreditkarte + SEPA-Lastschrift + PayPal + Klarna + giropay. Alles über Stripe (PayPal seit 2024 nativ unterstützt). PayPal wichtig als Vertrauenssignal (Käuferschutz) bei Erstkauf.
