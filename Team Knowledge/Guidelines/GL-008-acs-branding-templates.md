# GL-008 - ACS Branding Templates

> **This Guideline is a general rule every agent reads on every relevant action.** Any time a document or presentation is produced for the client/organization **ACS**, the specialist doing the work (Charta, Larry, or any future specialist) reads this Guideline first. It names the fixed template set ACS provides, where those templates live, and which one to start from for a given deliverable type.

> **This is not a token system.** Unlike [[GL-003-design-system]] (which Iris populates through a guided conversation to *derive* color/type/spacing tokens), ACS's branding arrived as six finished, pre-built Microsoft Office template files (`.dotm` / `.potm`). There is nothing to elicit — the brand decisions are already locked inside the files. Iris's job here is custodial: document what exists, where it lives, and the hard rule that governs its use. **GL-003 is untouched by this Guideline** — ACS branding does not feed the house design system; it stands alongside it as a client-specific asset set.

---

## 1. Who ACS is

ACS is a client/organization with its own fixed Microsoft Office branding — a set of six pre-made Word and PowerPoint templates supplied ready-to-use. myPKA does not design ACS's brand; myPKA **consumes** it, exactly as delivered, for every ACS deliverable.

*A corresponding CRM/Organizations entry for ACS may be needed in `PKM/CRM/Organizations/` — that is Penn's territory, not Iris's. Flagged for Larry to route separately; not created as part of this Guideline.*

---

## 2. Storage location

All six official ACS template files live at:

**`Team Knowledge/Guidelines/Assets/ACS-Branding/`**

These are the original binary Office files, moved as-is from `Team Inbox/` — not converted, not re-exported, not opened and re-saved. Byte-for-byte identical to what ACS supplied.

> **Move status: complete.** Larry moved the six files from `Team Inbox/` into `Team Knowledge/Guidelines/Assets/ACS-Branding/` on 2026-07-01 and staged them in git. The paths in this Guideline are the actual, current location.

---

## 3. The template set (six files)

| # | Filename | What it's for |
|---|---|---|
| 1 | `ACS bilingue_Carta intestata.dotm` | Bilingual (dual-language) letterhead Word template — for ACS correspondence that needs to read in two languages side by side or stacked. |
| 2 | `ACS_ITA_Carta intestata.dotm` | Italian-only letterhead Word template — standard ACS letterhead for Italian-language correspondence. |
| 3 | `DOC Informativi_Guideline_interna ACS-ITA.dotm` | Internal informational-document template (Italian) — for ACS-facing documents meant for internal circulation (guidelines, internal memos, internal policy notes). |
| 4 | `DOC Informativi_esterni ACS_ITA.dotm` | External informational-document template (Italian) — for ACS documents meant to leave the organization (client-facing or public informational content). |
| 5 | `Slide presentazione ACS_2026.potm` | PowerPoint presentation template, dated 2026 — the general-purpose ACS presentation deck shell (title, section, content, closing slides). |
| 6 | `Template_ACSOne_slide progetti.potm` | PowerPoint project-slide template for "ACSOne," a product of ACS — a single-slide format for presenting individual projects. |

*(File descriptions above are read from filenames only — the files themselves are binary Office templates and were not opened/parsed as text, per instruction. If any of these readings is wrong, correct it here and Iris will update.)*

---

## 4. The hard rule

**Any document or presentation produced for ACS MUST start from the matching template in this set. Never a from-scratch layout. Never a different brand's template — including myPKA's own house [[GL-003-design-system]] tokens.**

This applies to Charta (structured visual deliverables), Larry (if producing an ACS document directly), and any future specialist who ends up generating ACS-facing output. If none of the six templates fits the deliverable in hand, that is a **stop-and-ask** moment — flag it to Egon rather than improvising a look. ACS may need a seventh template commissioned from them, not invented by the team.

---

## 5. Deliverable-type -> template mapping (confirmed)

Egon confirmed this mapping as correct on 2026-07-01, with no corrections to any of the six rows. It is now the locked rule for which template a given ACS deliverable type starts from — still update-able if ACS's actual usage patterns diverge later, but not a proposal to revisit by default.

| Deliverable type | Start from | Why (inferred) |
|---|---|---|
| Formal external letter, Italian-only | `ACS_ITA_Carta intestata.dotm` | Named as the ITA letterhead; the default for single-language Italian correspondence. |
| Formal letter needing two languages (e.g. sent to a bilingual audience or with a parallel translation) | `ACS bilingue_Carta intestata.dotm` | Explicitly labeled "bilingue" (bilingual). |
| Internal ACS document — policy note, internal guideline, staff-facing informational doc | `DOC Informativi_Guideline_interna ACS-ITA.dotm` | Filename contains "interna" (internal). |
| External/client-facing informational document — fact sheet, public notice, external memo | `DOC Informativi_esterni ACS_ITA.dotm` | Filename contains "esterni" (external). |
| General client-facing or internal presentation deck | `Slide presentazione ACS_2026.potm` | Generic "presentazione" (presentation) naming, dated for current year — the default deck shell. |
| Single-slide project summary / one-pager for the ACSOne product | `Template_ACSOne_slide progetti.potm` | Named specifically for "slide progetti" (project slides), for ACSOne — confirmed by Egon as a product of ACS, not a sub-brand or project codename. |

**Flag to Egon:** confirm whether the 2026-dated presentation template (`Slide presentazione ACS_2026.potm`) needs to be swapped for a new year's version annually — if so, Iris should note an expected refresh cadence here. (The prior open question about ACSOne's nature is resolved: confirmed as a product of ACS.)

---

## 6. Relationship to GL-003

GL-003 remains the SSOT for myPKA's **own house** visual identity — the tokens Charta and Pixel use for deliverables that are not client-branded. GL-008 is a parallel, client-specific asset registry. When Charta produces something for ACS, GL-008 wins over GL-003; the ACS template dictates colors, type, and layout, not the house tokens. Iris does not attempt to reverse-engineer ACS's template into GL-003-style tokens — the templates are used wholesale, not decomposed.

---

## References

- [[GL-003-design-system]] — the house design-system SSOT; explicitly not touched by this Guideline.
- [[GL-001-file-naming-conventions]] — naming rules (this Guideline's own filename follows `GL-NNN-<slug>.md`; the six ACS template filenames are left unchanged from their original vendor names, which is an intentional exception since they are external assets, not myPKA-authored files).
- [[Team/Iris - Design System Architect/AGENTS]] — Iris's contract; author of this Guideline.
- [[Team/Charta - Infographic Designer/AGENTS]] — the specialist who will most often consume this Guideline when producing ACS deliverables.
