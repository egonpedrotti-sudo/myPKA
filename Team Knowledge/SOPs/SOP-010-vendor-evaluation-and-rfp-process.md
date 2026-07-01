# SOP-010 - Vendor Evaluation and RFP Process

- **Default owner:** Marlowe
- **Reusable by any agent.** This is a skill, not 1:1 ownership. Marlowe runs it most often; any specialist sourcing a vendor decision can invoke it.
- **Triggered by:** a sourcing event — new vendor selection, RFP, contract renewal, or re-negotiation.
- **References:** [[GL-006-confidential-vendor-data-handling]], [[GL-007-cost-tier-decision-framework]], [[GL-001-file-naming-conventions]]

## Purpose

Run a sourcing event the way world-class procurement operators do: never against vague requirements, never on price alone, always with a defensible weighted comparison, an enforceable SLA, and a tracked renewal date. This SOP exists to make the mediocre default — a spreadsheet of prices and a recommendation based on the lowest number — structurally unlikely.

## Procedure

### Phase 1 — Requirements, jointly owned

1. Confirm a requirements document exists before sourcing starts. If technical requirements (infrastructure, architecture, integration constraints) are missing or unclear, that is **not Marlowe's to invent.** Flag it as blocking and escalate to Egon directly — this is an open dependency until a Platform & Infrastructure specialist exists on the team (see [[Team/Marlowe - Senior Procurement Agent/AGENTS]] boundaries).
2. Confirm the commercial scope: budget ceiling, contract term length preference, must-have vs nice-to-have terms.
3. Do not proceed to Phase 2 against an undefined requirement. Sourcing against vague asks is the single most cited cause of procurement failure.

### Phase 2 — Weighted scoring criteria

1. Build a scoring rubric before any vendor is contacted or any quote is reviewed — never retrofit criteria to match a preferred vendor's strengths.
2. Weight criteria across at minimum: price (never the sole or dominant weight), total cost of ownership, contract terms (auto-renewal, termination rights, price-escalation caps), SLA quality, vendor stability/reputation, and integration/support fit as flagged by the requirements owner.
3. Document the weights before scores are entered. Weights fixed after seeing vendor responses invite post-hoc rationalization — the opposite of a defensible comparison.

### Phase 3 — TCO modeling (not price-only)

1. Model total cost of ownership, not sticker price. Include: base price, support-tier costs, overage/usage fees, integration/implementation cost, expected price escalation over the contract term, and switching cost if applicable.
2. Treat "lowest sticker price" as a red flag to interrogate, not a default winner — the lowest-price fallacy is the most commonly cited procurement failure mode across the field.
3. Redact vendor names and exact figures before consulting any external benchmark or market-rate source. See [[GL-006-confidential-vendor-data-handling]] — this is a hard gate, not optional.

### Phase 4 — SLA negotiation with named remedies

1. Negotiate service levels with named, enforceable remedies — service credits, termination rights, defined escalation paths — never aspirational uptime language with no consequence attached.
2. Every SLA clause in the term sheet should answer: "what happens if this is violated, concretely?" If the answer is nothing, the clause is decorative and needs to be renegotiated or flagged as a known gap.

### Phase 5 — Contract redline discipline

1. Redline the vendor's draft directly — track every changed clause, not just price. Priority redline targets: auto-renewal clauses, termination-for-convenience windows, price-escalation caps, audit rights.
2. For any clause requiring legal interpretation of enforceability, liability caps, indemnification, or regulatory compliance — **do not interpret it.** Flag it and hand to Legal. This is an open dependency: no Legal/Lex specialist exists on this team yet. Escalate to Egon directly rather than guessing at legal risk.
3. Keep the redlined draft and the vendor's original both in access-controlled storage per [[GL-006-confidential-vendor-data-handling]].

### Phase 6 — Renewal calendar discipline

1. Every contract entering this process gets a renewal calendar entry: the opt-out/renewal date and a lead-time trigger set **90-120 days before** that date. This window is what determines negotiating leverage — letting it lapse locks the organization into another term with zero leverage, the single most quoted procurement failure mode.
2. The lead-time trigger reopens this SOP at Phase 2 (rebuild or re-validate the scoring criteria — vendor landscape and internal needs may have shifted since the original sourcing event).
3. Renewal blindness (missing the auto-renewal window) is never acceptable. If a renewal date is discovered close to or past its lead-time window, flag it to Egon immediately as urgent, not as a routine update.

## Rigor discipline

Apply [[GL-007-cost-tier-decision-framework]]: RFP evaluation, TCO modeling, and redlines are Tier 3 work — full reasoning effort, show the weighting and the breakdown. Final legal veto, liability sign-off, or long-term vendor lock-in risk is Tier 4 — flag to Egon for human sign-off; do not finalize alone.

## Output / definition of done

A sourcing event run through this SOP is done when **all** of these exist:

- [ ] A vendor comparison matrix with weighted scoring criteria tied to the actual stated requirements.
- [ ] A TCO summary (one page, readable by a non-specialist in under five minutes) — not a price-only comparison.
- [ ] A negotiated term sheet redlining the vendor's draft with named clauses changed.
- [ ] An SLA with named, enforceable remedies.
- [ ] A renewal calendar entry with the opt-out date and the 90-120 day lead-time trigger recorded.
- [ ] Any technical-requirements gap or legal-interpretation gap flagged to Egon, not guessed at.
- [ ] All vendor-identifying and pricing detail redacted before any external research step, per [[GL-006-confidential-vendor-data-handling]].

If any of these are missing, the event is not done — it is the adequate-but-mediocre version this SOP exists to prevent.
