---
agent_id: iris
session_id: acs-branding-intake-2026-07-01
timestamp: 2026-07-01T14:00:00Z
type: mid-session-insight
linked_sops: []
linked_workstreams: []
linked_guidelines: ["GL-008-acs-branding-templates", "GL-003-design-system", "GL-001-file-naming-conventions"]
---

# ACS branding templates — new client-specific asset registry (GL-008), GL-003 untouched

## Context

Larry routed a Team Inbox drop: Egon placed six pre-made Microsoft Office branding template files (`.dotm` Word templates, `.potm` PowerPoint templates) for a client/organization called ACS into `Team Inbox/`. Instruction: use those templates, unchanged, as the mandatory basis for any future ACS document or presentation. This is not a "populate GL-003" request — it's a finished, external, pre-branded asset set that needs a home and a usage rule, not a token-elicitation session.

## What we did

- Iris authored a new Guideline, `Team Knowledge/Guidelines/GL-008-acs-branding-templates.md`, documenting: who ACS is (a client with a fixed Office branding set), the intended storage location (`Team Knowledge/Guidelines/Assets/ACS-Branding/`), the six files and what each is for (read from filenames only — files were not opened/parsed, per instruction), the hard rule that any ACS deliverable must start from the matching template and never a from-scratch layout or a different brand's tokens, and an inferred deliverable-type -> template mapping table flagged as unconfirmed.
- Iris added a GL-008 row to `Team Knowledge/Guidelines/INDEX.md` and bumped "Next free Guideline slot" from GL-008 to GL-009.
- Iris explicitly did **not** touch [[GL-003-design-system]] — GL-008 is a parallel, client-specific registry; GL-003 remains the house design system for non-client-branded work.
- Iris did **not** create a `PKM/CRM/Organizations/` entry for ACS — flagged in GL-008 §1 for Penn/Larry to handle, per Iris's contract (Iris does not write into PKM/ or entity folders).

## Decisions made

- **Question:** Should ACS's branding be reverse-engineered into GL-003-style color/type/spacing tokens?
  **Decision:** No. The templates are used wholesale, as delivered. GL-008 explicitly states Iris does not decompose them into tokens — that would risk drift from the actual Office files, which are the real SSOT for ACS-branded output.
- **Question:** Where do finished, non-token brand assets like this live going forward?
  **Decision:** `Team Knowledge/Guidelines/Assets/<client-or-topic>/` — a new pattern (this is the first entry). Sibling Guidelines pointing at future non-token brand asset sets should follow the same `Assets/<slug>/` convention under Guidelines.

## Insights

- Not every brand-relevant input fits Iris's usual guided-conversation authoring pattern. When the input arrives as finished, external, binary artifacts (not values to elicit from the user), the correct move is a custodial Guideline — document, locate, rule, don't decompose. This is a durable pattern worth watching for reuse if more clients/orgs hand over pre-made brand kits.
- **Toolset gap surfaced this session:** Iris's available tools in this session (Read, Write, Edit, Glob, Grep) included no Bash/shell tool, so the required `git mv` of the six binary template files from `Team Inbox/` to `Team Knowledge/Guidelines/Assets/ACS-Branding/` could **not** be executed by Iris directly. The exact `git mv` commands are documented in GL-008 §2 for Larry (or any agent with shell access) to run. This is flagged clearly in GL-008 itself so no downstream agent assumes the move already happened.

## Realignments

- _(none this session — this was a routed task, not a course correction)_

## Open threads

- [ ] **BLOCKING:** Run the six `git mv` commands documented in `GL-008-acs-branding-templates.md` §2 to actually relocate the files from `Team Inbox/` to `Team Knowledge/Guidelines/Assets/ACS-Branding/`. Iris had no shell access this session.
- [ ] Egon to confirm or correct the inferred deliverable-type -> template mapping table in GL-008 §5 (letter type, internal-vs-external doc, which presentation template for which use case).
- [ ] Egon to confirm whether "ACSOne" is a distinct ACS sub-brand/program or a project codename (affects how `Template_ACSOne_slide progetti.potm` gets used going forward).
- [ ] Egon to confirm whether `Slide presentazione ACS_2026.potm` needs an annual refresh/replacement cadence.
- [ ] Larry/Penn to consider a `PKM/CRM/Organizations/` entry for ACS (Iris does not create entity notes).

## Next steps

- Once the `git mv` runs, update GL-008 §2's "Move status" note from pending to complete.
- Charta reads GL-008 before producing any ACS-facing deliverable going forward.

## Cross-links

- _(no prior ACS-related session log exists yet — this is the first)_
