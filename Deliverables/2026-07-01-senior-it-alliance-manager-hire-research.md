# Hire Research Brief: Senior IT Alliance Manager

**Requested by:** Nolan, per [[SOP-001-how-to-add-a-new-specialist]] Step 2.
**Researcher:** Pax.
**Scope given:** managing strategic vendor relationships (VMware-style ISVs, cloud providers, hardware OEMs), tracking partner tiers/benefits, navigating ecosystem/program changes, handling vendor escalations.

## 1. What world-class looks like, day to day

The best alliance managers run a "rhythm of business" with each strategic vendor: recurring business reviews, a live map of partner-tier requirements versus current standing, and a named escalation contact per vendor rather than a generic support queue (Confidence: **High** — ZINFI's alliance-manager glossary and flashdba's hyperscaler-GTM writeup independently converge on this cadence-plus-named-contact model). Day to day, this looks like: tracking certification/badge requirements that keep the org's partner tier current, monitoring vendor program-change announcements before they become a surprise, maintaining a relationship map (who at the vendor owns what), and triaging escalations by severity rather than routing everything to the same channel.

The most consequential recent case study for exactly this role: Broadcom's post-acquisition overhaul of the VMware partner ecosystem. Independently reported by Channel Dive, IT Pro, Virtualization Review, and ChannelInsider — all converge on the same facts: Broadcom terminated the legacy reseller/solution-provider programs in early 2024, moved existing partners onto an invitation-only Advantage Partner Program, eliminated the bottom partner tier while raising eligibility bars on the remaining tiers, and in 2025 further cut the VMware Cloud Service Provider partner roster (non-invited partners received non-renewal notices in July 2025, with a transact-only window through October 2025). This is a textbook example of the exact "ecosystem/program change navigation" this role must own — a world-class alliance manager would have flagged the tier-eligibility shift and invitation risk to leadership well before a non-renewal notice arrived, not after (Confidence: **High**, multi-source corroborated).

## 2. Core competencies and anti-patterns

**Competencies:**
- Program literacy: actively tracks partner-tier requirements (certifications, revenue commitments, points-based badge systems) rather than treating tier status as a fixed fact — VMware's TAP program alone has three tiers (Standard/Advanced/Strategic) with badge-based advancement, independently documented by VMware's own TAP materials and TechTarget's partner-network explainer.
- Escalation routing discipline: named owners per vendor, not team-wide paging — the inverse of the anti-pattern documented industry-wide in incident-response escalation design (incident.io), which transfers directly to vendor-escalation practice per Sequential Tech's telecom-vendor-escalation writeup.
- Relationship health tracking distinct from commercial tracking — alliance value shows up in roadmap access, co-sell motion, and early warning on program change, not just discount percentage.
- Ecosystem-change radar: monitoring vendor partner-program announcements as a standing task, not a reactive one.

**Anti-patterns (explicitly avoid):**
- **Alliance-as-marketing-adjunct.** The most commonly cited failure mode: alliance function gets bolted onto product marketing and produces joint webinars and conference booths with no actual pipeline or program-risk tracking — explicitly documented as a common anti-pattern by flashdba's cloud-alliances analysis.
- **Reactive-only posture.** Learning about a partner-tier demotion or program termination from a notification email instead of tracking eligibility requirements proactively — this is precisely what the Broadcom/VMware case study punishes; multiple sources document partners caught flat-footed by short transition windows.
- **Escalation chain sprawl.** Overly deep chains, paging whole teams instead of named owners, stale routing tied to org charts nobody re-checked — documented as a general escalation anti-pattern (incident.io) that applies just as much to vendor relationships as internal incident response.
- **Treating "relationship" as purely social.** Golf-and-dinners alliance management with no tracked deliverable, no scorecard, and no early-warning system is the generic, low-value version of this role.
- **Conflating alliance management with procurement.** An alliance manager who starts negotiating commercial terms directly duplicates and undermines the Procurement role — see boundary below.

## 3. Deliverables

World-class output: a live partner-tier scorecard (current tier, requirements to maintain/advance it, renewal/certification deadlines), an escalation log with named vendor contacts and resolution SLAs, a standing "ecosystem watch" brief flagging upcoming program changes before they hit (the Broadcom precedent is the model case for what this should have caught), and pre-negotiation partnership-value context handed to Procurement ahead of any commercial renewal (not the negotiation itself).

Adequate-but-mediocre output: a contact list, a folder of vendor PDFs, and reactive escalation emails with no tracked pattern or tier awareness. This is what a generic AI-flavored "vendor relationship manager" produces by default — no proactive monitoring, no distinction between relationship health and commercial terms.

## 4. Boundaries

- **Holds:** partner-tier tracking, relationship health, escalation triage and routing, ecosystem/program-change monitoring, vendor roadmap and co-sell intelligence.
- **Refuses / hands back:** commercial negotiation, pricing, licensing structure, contract redlines — these belong to the Senior Procurement Agent (see companion brief, `[[2026-07-01-senior-procurement-agent-hire-research]]`). The Alliance Manager feeds partnership context *into* Procurement's negotiation; does not negotiate terms directly.
- **Refuses:** final strategic decisions on vendor selection, program participation, or acquisition-driven exit/stay calls. The brief given for this role names "CTO" and "Procurement" as collaborators — **the CTO role does not exist on this team.** Egon fills that decision-making seat directly. This is an **open dependency to flag, not resolve**: the Alliance Manager's contract should route final-call escalations to Egon by default, not assume a CTO seat exists.
- **Refuses:** legal interpretation of partner-program terms (e.g., whether a program change breaches an existing commitment) — hands to **Lex** (Legal), an anticipated-but-not-yet-hired role already referenced in Vex's contract as a relevant existing thread.
- **Confidential-data discipline (critical, given commercial/contractual documents handled):** World-class practice treats partner-tier standing, non-public roadmap briefings (frequently under NDA at strategic/technology-alliance tiers), and vendor-specific discount or rebate structures as protected — never pasted into public research tools or unsecured channels when benchmarking against other vendors' programs. Sloppy version: quoting a vendor's confidential roadmap slide or rebate structure verbatim into an external search/LLM query "to compare against competitor X's program" — a direct NDA violation risk, independently consistent with the NDA-handling norms found in procurement's confidentiality practice (Ironclad, Vendor Centric) and directly transferable here since strategic/technology-alliance materials are routinely NDA-gated. Good version: describes program mechanics in generic terms ("Vendor's top tier requires X certifications") without quoting the vendor's own confidential deck, and keeps any NDA'd roadmap material in access-controlled storage, never in a shared research doc.

## 5. Name candidates

Short, single-word, no collision with Larry, Nolan, Pax, Penn, Mack, Silas, Felix, Vex, Vera, Iris, Charta, Pixel:

- **Ansel** — neutral, professional, evokes steady relationship stewardship.
- **Rowan** — distinct, no collisions, slightly warmer tone fitting relationship-management work.
- **Casca** — short, distinct; avoid if it reads too adjacent to "Charta."
- **Dorian** — distinct, no collisions.
- **Bren** — short, crisp, no collisions.

Note: keep this name phonetically distinct from "Vex," "Vera," and "Pax" (the team already has three short V/P-heavy names) to reduce voice-routing ambiguity for Larry.

## Cross-cutting note for Nolan

Both roles in this hiring round handle confidential commercial/financial/contractual material and should share one operating-discipline clause rather than two independently drafted ones — consider drafting this as a shared Guideline (e.g., a `GL-00X-confidential-vendor-data-handling` covering redaction-before-external-research, no-paste-into-shared-or-insecure-channels, and access-controlled storage of unredacted originals) that both contracts reference via `[[wikilink]]`, per the SSOT Golden Rule, rather than duplicating the same red-flag protocol into both `AGENTS.md` files.
