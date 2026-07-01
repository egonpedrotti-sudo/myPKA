# GL-006 - Confidential Vendor Data Handling

> **This Guideline is a general rule every agent reads on every relevant action.** Where more than one specialist handles commercial, financial, or contractual vendor material, the redaction and storage discipline lives here once. SOPs and contracts `[[wikilink]]` to this file rather than restating the rule.

This is the source of truth for how anyone on the team — currently **Marlowe** (Senior Procurement Agent) and **Ansel** (Senior IT Alliance Manager), and any future specialist who touches vendor, partner, or supplier material — handles confidential commercial data. Vendor pricing, discount tiers, rebate structures, non-public roadmap material, and draft contract language are routinely NDA-bound. Mishandling them is not a hygiene lapse; it can be a contract breach.

## The core rule

**Redact before it leaves a controlled context. Every time. No exceptions for convenience.**

A controlled context is: the deal's own NDA'd parties, and access-controlled storage the user already controls. Anything else — an external search query, a public LLM chat, a shared Slack channel, an unencrypted scratch file, a general research note — is an uncontrolled context by default.

## What counts as sensitive

- Vendor names tied to specific pricing, discount percentages, or rebate structures.
- Unit pricing, account-specific discount tiers, and negotiated rate figures.
- Draft or executed contract language not yet finalized.
- Non-public partner-program terms, roadmap briefings, or tier-eligibility criteria shared under NDA.
- Any figure or clause whose disclosure outside the deal's named parties would itself breach an NDA.

## The STOP rule (mandatory, no override)

If you detect un-anonymized or un-redacted sensitive commercial, financial, or legal data about to leave a controlled context — about to be pasted into an external search or LLM query, written into a shared document, or saved somewhere without access control — **STOP immediately.** Do not proceed until the data is redacted or anonymized in place. This is not a suggestion to consider; it is a hard gate. There is no local-model or automated redaction step in this scaffold — redaction is something you, the agent, do inline, by hand, before the content moves anywhere.

Concretely:

1. Recognize the pattern (vendor name + price, vendor name + discount %, quoted contract clause, quoted roadmap language) before you act, not after.
2. Rewrite in place: vendor names become `Vendor A` / `Vendor B`; exact figures become ranges or order-of-magnitude bands; quoted language becomes a generic paraphrase of the mechanic ("Vendor's top tier requires N certifications") rather than a verbatim excerpt.
3. Only then continue with the external research, comparison, or write.
4. If you cannot redact without destroying the value of the research (the specific figure *is* the question), say so and ask Egon directly instead of proceeding un-redacted.

## Good version vs sloppy version

- **Sloppy:** pasting a raw vendor quote — company name and discount percentage visible — into a public search tool or LLM chat "to get a second opinion" or benchmark against market rate.
- **Good:** "Vendor A quoted a per-seat rate in the mid-tier band for a 3-year term with an auto-renewal clause — how does that compare to typical market terms for this category?" No name, no exact figure, no verbatim clause.

- **Sloppy:** quoting a vendor's confidential roadmap slide or rebate structure verbatim into an external query "to compare against competitor X's program."
- **Good:** "Vendor's top partner tier requires a revenue commitment and a points-based certification count" — the mechanic, not the deck.

## Storage discipline

- Unredacted originals (the actual signed contract, the actual vendor quote, the actual NDA'd roadmap deck) live only in access-controlled storage the user already controls outside of shared or public channels.
- Working notes, comparison matrices, and research artifacts that will be shared, discussed externally, or handed to Egon for a quick read use the redacted form by default.
- If unredacted material must be referenced in a `Deliverables/` artifact, keep it in a section clearly marked as controlled and confirm with Egon before it's shared any wider than the current conversation.

## Applies to

- **[[Team/Marlowe - Senior Procurement Agent/AGENTS]]** — vendor quotes, contract redlines, TCO models, RFP responses.
- **[[Team/Ansel - Senior IT Alliance Manager/AGENTS]]** — partner-tier standing, NDA'd roadmap briefings, rebate/discount structures.
- **[[SOP-010-vendor-evaluation-and-rfp-process]]** and **[[SOP-011-partner-tier-tracking-and-escalation-management]]** — both reference this Guideline instead of restating the rule.
- Any future specialist who handles vendor, partner, or supplier material.

## Updates to this Guideline

If the discipline changes, update this file. Do not duplicate the rule into either contract or either SOP. They `[[wikilink]]` here and inherit the change automatically.

## References

- [[GL-001-file-naming-conventions]]
- [[Team/Marlowe - Senior Procurement Agent/AGENTS]]
- [[Team/Ansel - Senior IT Alliance Manager/AGENTS]]
- [[SOP-010-vendor-evaluation-and-rfp-process]]
- [[SOP-011-partner-tier-tracking-and-escalation-management]]
