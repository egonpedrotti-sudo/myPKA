# SOP-011 - Partner-Tier Tracking and Escalation Management

- **Default owner:** Ansel
- **Reusable by any agent.** This is a skill, not 1:1 ownership. Ansel runs it most often; any specialist managing a strategic vendor relationship can invoke it.
- **Triggered by:** onboarding a new strategic vendor relationship, a recurring rhythm-of-business cadence, a vendor escalation, or a vendor program-change announcement.
- **References:** [[GL-006-confidential-vendor-data-handling]], [[GL-007-cost-tier-decision-framework]], [[GL-001-file-naming-conventions]]

## Purpose

Run strategic vendor relationships the way world-class alliance managers do: a standing rhythm of business, a live scorecard of tier requirements versus current standing, named escalation contacts instead of a generic support queue, and proactive monitoring of ecosystem/program change before it becomes a surprise. This SOP exists to make the mediocre default — a contact list, a folder of vendor PDFs, and reactive escalation emails — structurally unlikely.

## Procedure

### Phase 1 — Rhythm of business

1. For every strategic vendor relationship (ISVs, cloud providers, hardware OEMs), establish a recurring business-review cadence rather than ad hoc contact. Cadence frequency scales with relationship strategic weight — set it explicitly, don't leave it implicit.
2. Maintain a relationship map: who at the vendor owns what (technical contact, commercial contact, escalation contact, executive sponsor if one exists).
3. Alliance management that produces only joint webinars and conference booths with no tracked deliverable or program-risk awareness is the marketing-adjunct anti-pattern — explicitly avoid it. Every relationship in this SOP has a tracked scorecard, not just a social calendar.

### Phase 2 — Partner-tier scorecard

1. Build and maintain a live scorecard per vendor: current partner tier, the requirements to maintain or advance it (certifications, revenue commitments, points/badge thresholds), and the renewal/certification deadlines attached to those requirements.
2. Treat tier status as something that must be actively tracked, not a fixed fact set once at onboarding. Program requirements change; badge and certification thresholds shift; revisit the scorecard on the same cadence as the business review.
3. Redact vendor-specific rebate structures, discount tiers, and any NDA'd roadmap content before this scorecard is shared outside its controlled storage location. See [[GL-006-confidential-vendor-data-handling]].

### Phase 3 — Escalation triage and named-contact discipline

1. Every vendor relationship has a **named escalation contact**, not a generic support-queue routing. Document who that is and keep it current — stale routing tied to an org chart nobody re-checked is a documented anti-pattern.
2. Triage escalations by severity. Route by severity to the appropriate named contact rather than paging broadly or defaulting every issue to the same channel.
3. Maintain an escalation log: what happened, who was contacted, the resolution SLA, and the actual resolution time. Patterns across this log (repeated escalations to the same vendor, missed resolution SLAs) are themselves a signal worth surfacing proactively, not just a record.

### Phase 4 — Ecosystem-change radar

1. Monitor each strategic vendor's partner-program announcements as a standing task — a recurring check, not a reactive one triggered only when something breaks.
2. Watch specifically for: tier-eligibility changes, program terminations or restructures, invitation-only transitions, and non-renewal notice windows. The reference case for exactly this failure mode: Broadcom's 2024-2025 overhaul of the VMware partner ecosystem, where legacy reseller programs were terminated, partners were moved onto an invitation-only tier, the bottom tier was eliminated, and non-invited Cloud Service Provider partners received non-renewal notices in July 2025 with only a transact-only window through October 2025. A world-class alliance manager flags a tier-eligibility shift and invitation risk **before** a non-renewal notice arrives — this SOP's Phase 4 exists specifically to catch that pattern early instead of after the fact.
3. Produce a standing "ecosystem watch" brief per strategic vendor, updated when program-change signals appear, not only at renewal time.

### Phase 5 — Handoff to Procurement

1. When a commercial renewal or negotiation is approaching, hand partnership-value context — relationship health, tier standing, roadmap/co-sell intelligence — to **Marlowe** (Senior Procurement Agent) ahead of the negotiation. Ansel feeds context into the negotiation; Ansel does not negotiate commercial terms directly. Negotiating terms is Marlowe's boundary, not Ansel's.
2. For final strategic decisions on vendor selection, program participation, or an acquisition-driven exit/stay call, escalate to Egon directly. No CTO seat exists on this team; do not assume one, do not invent a placeholder — Egon fills that decision-making seat.

## Rigor discipline

Apply [[GL-007-cost-tier-decision-framework]]: partner-tier scorecards and escalation-pattern analysis are Tier 3 work — full reasoning effort, show the tier-requirement gap explicitly. An ecosystem-change event with strategic-lock-in or exit/stay consequence (the Broadcom/VMware pattern) is Tier 4 — flag to Egon for human sign-off; do not finalize the strategic call alone.

## Output / definition of done

A vendor relationship managed through this SOP is current when **all** of these are true:

- [ ] A live partner-tier scorecard exists: current tier, requirements to maintain/advance it, renewal/certification deadlines.
- [ ] A named escalation contact is documented and current, not a stale or generic routing.
- [ ] An escalation log tracks resolution SLAs and actuals, not just a running list of emails.
- [ ] A standing ecosystem-watch brief exists per strategic vendor and has been updated within the current business-review cadence.
- [ ] Any pending commercial renewal has partnership-value context already handed to Marlowe before the negotiation starts.
- [ ] Any final vendor-selection, program-participation, or exit/stay call is flagged to Egon rather than decided unilaterally.
- [ ] All NDA'd roadmap material and rebate/discount detail is redacted before appearing outside controlled storage, per [[GL-006-confidential-vendor-data-handling]].

If any of these are missing, the relationship is running the adequate-but-mediocre version this SOP exists to prevent.
