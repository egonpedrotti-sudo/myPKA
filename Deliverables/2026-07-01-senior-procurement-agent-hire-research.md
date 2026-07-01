# Hire Research Brief: Senior Procurement Agent

**Requested by:** Nolan, per [[SOP-001-how-to-add-a-new-specialist]] Step 2.
**Researcher:** Pax.
**Scope given:** vendor evaluation, cost optimization, hardware/software RFPs, SLA definition, financial contract negotiations. Boundary: commercial terms, licensing structures, budgets — not technical requirements gathering.

## 1. What world-class looks like, day to day

The best procurement operators split time between two modes: **cadence work** (spend analysis, renewal calendars, vendor scorecards) and **event work** (RFPs, negotiations, escalations). World-class procurement starts every sourcing event with a requirements document owned jointly with a technical stakeholder — never sources against vague asks, because ill-defined requirements are the single most cited cause of procurement failure (Confidence: **High** — corroborated independently by Spendflo's 2026 procurement guide and NPI Financial's IT procurement best-practices writeup, both naming "starting sourcing without defined requirements" as the top failure mode). For renewals, the best operators run a 90-120 day lead calendar before contract opt-out dates, because that window is what determines negotiating leverage (Confidence: **High** — Vertice and NPI Financial independently converge on the 90-120 day figure). Day to day, this looks like: maintaining a rolling contract/renewal tracker, running total-cost-of-ownership models (not just sticker price), negotiating SLAs with named remedies (credits, termination rights) rather than aspirational uptime language, and building vendor scorecards that feed back into renewal leverage.

## 2. Core competencies and anti-patterns

**Competencies:**
- TCO modeling that includes hidden costs (support tiers, overage fees, integration cost) — evidenced by the "lowest price fallacy" being independently named as a core failure by Tradogram and NPI Financial.
- Contract literacy: reading auto-renewal clauses, termination-for-convenience windows, price-escalation caps, and audit rights before signature — critical given that ~89% of SaaS contracts now carry auto-renewal clauses (Confidence: **Medium** — single-study figure from Vertice, not independently replicated, but directionally consistent with Zylo's SaaS-sprawl reporting).
- Vendor consolidation discipline — recognizing that too many vendors dilutes negotiating power (Tradogram; corroborated qualitatively by Spendflo).
- SLA definition with enforceable remedies, not decorative KPIs.

**Anti-patterns (explicitly avoid):**
- **Price-only sourcing.** Awarding to the lowest bidder without TCO or risk-adjustment. Independently flagged by Tradogram and NPI Financial as the most common and most costly procurement mistake.
- **Adversarial-only negotiation.** Treating every vendor interaction as zero-sum; this is documented as the outdated model the best procurement orgs have moved away from in favor of value-based negotiation that still holds firm boundaries.
- **Renewal blindness.** Letting auto-renewal windows lapse, which locks the organization into another term at a worse price with zero leverage — the single most quoted 2025-2026 procurement failure across every source consulted.
- **Generic RFP templates with no weighted scoring criteria.** Produces vendor comparisons that can't be defended later and invite post-hoc rationalization.
- **Negotiating alone on technical scope.** A procurement agent who tries to also define technical requirements either over-scopes (inventing specs it isn't qualified to set) or under-scopes (accepting the vendor's own framing of what's needed) — this is exactly why the role's boundary must hold (see §4).

## 3. Deliverables

World-class output: a vendor comparison matrix with weighted scoring criteria tied to actual stated requirements, a negotiated term sheet redlining the vendor's draft with named clauses changed (not just price), a renewal calendar entry with the opt-out date and lead-time trigger, and a one-page TCO summary that a non-specialist (Egon) can approve in under five minutes.

Adequate-but-mediocre output: a spreadsheet of vendor prices with a recommendation based on lowest number, no SLA redlines, no renewal date tracked, no TCO breakdown. This is the default output of a generic AI-flavored procurement assistant — Nolan should design against it explicitly.

## 4. Boundaries

- **Holds:** commercial terms, licensing structure, cost modeling, RFP process, SLA negotiation, contract redlines, vendor scorecards, renewal calendar ownership.
- **Refuses / hands back:** technical requirements definition (what infrastructure, what architecture, what integration constraints) — this belongs to a **Platform & Infrastructure specialist role that does not yet exist on this team.** This is an **open dependency**: until that role is hired, the Procurement specialist either escalates technical-requirements gaps to Egon directly or flags them as blocking, rather than guessing at technical specs itself. Nolan should note this gap in the contract rather than paper over it.
- **Refuses:** legal interpretation of contract enforceability, liability caps, indemnification language, regulatory compliance clauses — hands to **Lex** (Legal), an anticipated-but-not-yet-hired role already referenced in Vex's contract. Same open-dependency pattern as above; flag, don't invent.
- **Confidential-data discipline (critical, given commercial/financial documents handled):** World-class practice redacts vendor names, unit pricing, and account-specific discount tiers *before* using any external tool, benchmark service, or search query to research market rates — because vendor pricing is typically NDA-bound confidential information, and pasting it into an unredacted external channel is a contract breach, not just a hygiene lapse (Confidence: **High** — independently corroborated by Ironclad's and Vendor Centric's NDA-handling guidance, both naming pricing/discount data as the paradigm case of protected information). Sloppy version: pastes raw vendor quotes (with company names and discount percentages visible) into a public LLM chat, a shared Slack channel, or an unencrypted spreadsheet to "get a second opinion" or benchmark pricing — this is the single most avoidable and most damaging failure mode for this role, since it can trigger actual contractual liability, not just an internal process gripe. Good version: strips identifying details to "Vendor A / Vendor B," uses ranges instead of exact figures when consulting anything outside the deal's own NDA'd parties, and keeps unredacted originals only in access-controlled storage.

## 5. Name candidates

Short, single-word, no collision with Larry, Nolan, Pax, Penn, Mack, Silas, Felix, Vex, Vera, Iris, Charta, Pixel:

- **Marlowe** — evokes negotiation and dealmaking without being on-the-nose.
- **Cato** — historically associated with fiscal scrutiny and austerity; short, distinct.
- **Odell** — neutral, professional, no collisions.
- **Quill** — evokes contract redlining and paperwork precision.
- **Bram** — short, distinct, no obvious associative baggage either way.

Nolan's pick should favor something that doesn't imply legal authority (avoid names that read as "the lawyer") since Lex is reserved for that seat later.
