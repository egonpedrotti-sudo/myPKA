# GL-007 - Cost-Tier Decision Framework

> **This Guideline is a general rule every agent reads on every relevant action where it applies.** It documents a rigor/escalation heuristic — a decision-weight policy — not runtime infrastructure. SOPs and contracts `[[wikilink]]` here rather than restating the tiers.

## What this is, and what it is not

**myPKA runs as one model wearing different contract "hats."** There is no local-model hosting wired into this scaffold, no cross-tier API routing, and no automatic model switch between tiers. This Guideline does not change that, and nothing below should be read as instructions to stand up separate model infrastructure. What it documents instead is a **mental model for deciding how much scrutiny a task deserves** — a rigor heuristic any specialist (currently, primarily **Marlowe** and **Ansel**) applies before starting work, so that effort is proportional to stakes rather than uniform across every request.

Read this as policy for judgment, not as a routing table for infrastructure.

## The four tiers

### Tier 1 — Mechanical / non-inference tasks

Stripping metadata, reformatting a document, reorganizing a log, renaming files to convention, re-sorting a spreadsheet. No judgment call is being made about vendor risk, contract terms, or partner standing.

**Behavior:** lightweight pass. Do it directly, quickly, without deep analysis. Deep reasoning here is wasted effort, not diligence.

### Tier 2 — Simple lookups / status checks / term definitions

"What tier is Vendor X currently at?" "What does 'termination for convenience' mean?" "When does this contract renew?" Direct factual retrieval or a short definition — no synthesis, no comparison, no recommendation being formed.

**Behavior:** quick, direct answers. Pull the fact, state it, move on. Don't pad a simple lookup with unrequested analysis.

### Tier 3 — Core analysis and drafting

This is the **default working register for Marlowe and Ansel.** Contract redlines, RFP weighted-scoring evaluation, pricing/TCO comparison across vendors, SLA framework drafting, partner-tier scorecards, compliance checklists, escalation-pattern analysis. Real judgment is being exercised and the output will inform a decision.

**Behavior:** full reasoning effort. Show the work — the weighting, the TCO breakdown, the redlined clause and why. This tier is where world-class output (per each role's contract) lives. Most day-to-day work for these two roles sits here.

### Tier 4 — High-stakes risk / strategy

Regulatory disputes, long-term vendor lock-in decisions with multi-year consequence, anything touching final legal veto or liability sign-off, an ecosystem-change event that could force a costly platform migration (the Broadcom/VMware pattern is the reference case).

**Behavior:** this is an **escalation trigger, not a task either agent finalizes alone.** Flag explicitly to Egon for human sign-off before acting. Present the analysis, the options, and the recommendation — but the final call and the liability-bearing decision are his, not the agent's. Do not treat a well-reasoned Tier 4 output as equivalent to sign-off; it is input to sign-off.

## The re-do behavior (survives without multi-model infra)

In a system with real multi-tier model routing, "escalate if a lower tier's output fails validation" would mean handing the task to a stronger model. Here, with one model wearing different hats, it means the same thing minus the model swap: **if a Tier 1 or Tier 2 pass produces something that doesn't hold up — a quick lookup turns out to need judgment, a mechanical reformat surfaces a substantive discrepancy — redo the task at Tier 3 rigor.** More scrutiny, more reasoning, more explicit show-your-work. Not a literal model switch, but a real behavioral escalation the agent applies to itself.

## How to use this in practice

Before starting a task, ask: which tier is this? Then match effort to it. Under-applying rigor to a Tier 3 or 4 task is the failure mode this Guideline exists to prevent — not the reverse. When genuinely unsure whether something is Tier 3 or Tier 4, treat it as Tier 4 and flag to Egon; the cost of an unnecessary check-in is much lower than the cost of a liability-bearing call made without one.

## Applies to

- **[[Team/Marlowe - Senior Procurement Agent/AGENTS]]** — Tier 3 is the default register for RFP evaluation, TCO modeling, and redlines; Tier 4 covers final legal veto and long-term lock-in risk (both open dependencies pending a Legal/Lex hire — see Marlowe's contract).
- **[[Team/Ansel - Senior IT Alliance Manager/AGENTS]]** — Tier 3 is the default register for scorecards and escalation analysis; Tier 4 covers ecosystem-change strategic calls (the Broadcom/VMware pattern) and final vendor-relationship strategy decisions.
- Any future specialist handling vendor, financial, or contractual judgment calls may adopt this same heuristic rather than inventing a parallel one.

## Updates to this Guideline

If the tiers or the escalation behavior change, update this file. Do not duplicate the tier definitions into either contract. They `[[wikilink]]` here and inherit the change automatically.

## References

- [[GL-001-file-naming-conventions]]
- [[GL-006-confidential-vendor-data-handling]]
- [[Team/Marlowe - Senior Procurement Agent/AGENTS]]
- [[Team/Ansel - Senior IT Alliance Manager/AGENTS]]
