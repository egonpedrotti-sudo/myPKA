---
title: Broadcom/VMware Alternatives — Board Deck Content Plan
date: 2026-07-01
author: Charta (Infographic Designer)
purpose: Slide-by-slide content/design plan for Egon's board presentation to ACS's board. Larry assembles the actual .pptx against the ACS template mechanically from this plan.
status: plan-for-assembly — content sourced from [[2026-07-01-broadcom-vmware-alternatives-brief]] (Ansel); time-sensitive figures flagged for re-verification before the board meeting
source_brief: "Deliverables/2026-07-01-broadcom-vmware-alternatives-brief.md"
template: "Team Knowledge/Guidelines/Assets/ACS-Branding/Slide presentazione ACS_2026.potm"
branding_guideline: "[[GL-008-acs-branding-templates]]"
slide_count: 6
---

# Broadcom/VMware Alternatives — Board Deck Content Plan

## Branding note (read first)

This deck is for ACS's board and MUST be built from `Team Knowledge/Guidelines/Assets/ACS-Branding/Slide presentazione ACS_2026.potm` per [[GL-008-acs-branding-templates]] — the general-purpose ACS presentation deck shell (title, section, content, closing slides). **GL-008 overrides [[GL-003-design-system]] entirely for this deliverable**: no house color/type/spacing tokens are used anywhere in this plan. All colors, fonts, and layout masters come wholesale from the .potm's built-in slide masters. Charta is not decomposing the template into tokens — every "layout type" cited below refers to whichever master/layout inside the .potm most closely matches that description (title, section header, content/bullets, comparison/table, closing). Larry (or whoever assembles the .pptx) should pick the nearest matching master inside the template rather than inventing a new one; if no master fits a given slide, that's a stop-and-ask back to Egon per GL-008 §4, not an improvised layout.

GL-003 itself is currently unpopulated (placeholder-only) — irrelevant here since GL-008 wins for ACS work, but flagged per Charta's standing discipline in case a future non-ACS deliverable needs it.

## Brief-to-deck mapping

Ansel's brief maps almost 1:1 to a 5-slide arc plus an optional closing slide. Egon asked for "poche slide di alto livello" — this plan holds to **6 slides total**, each scoped to fit on one screen with no walls of text. The arc below follows the suggested structure with one adjustment: the brief's §4 (Recommendation Shape) is split conceptually across slide 5 (next steps) so the "shortlist + RFP + pilot" sequence reads as one clear action, and a short closing slide is added since board decks conventionally end on an explicit "what we're asking you to approve" + questions beat rather than trailing off after the last content slide.

---

## Slide 1 — Title / Cover

**Layout type:** Title slide (ACS template title master)

**Purpose / one-line takeaway:** Frame the topic and who's presenting — the board should immediately know what decision-adjacent topic this is and that it's a briefing, not a vote.

**Content:**
- Title: **"VMware/Broadcom: Navigating the Licensing Shift"** *(or Egon's preferred Italian/English phrasing — confirm language with Egon; brief and this plan are in English, but ACS board decks may run Italian — flag to Egon before assembly)*
- Subtitle: "Alternatives landscape and recommended next step"
- Presenter line: Egon (or whoever presents), date of board meeting
- No body content beyond title/subtitle/presenter/date — title slides in the ACS master carry minimal text by convention

---

## Slide 2 — The Trigger: Why This Is on the Agenda Now

**Layout type:** Bullet content slide

**Purpose / one-line takeaway:** Broadcom's acquisition of VMware has permanently changed the licensing model — this is an active, ongoing disruption, not a settled one-time shock, and it directly affects ACS's cost and vendor risk.

**Content (4 bullets max, board-level, no engineering detail):**
- Perpetual VMware licenses are gone — subscription-only since Feb 2024, sold in large bundles (VMware Cloud Foundation) priced per core, not per socket
- New minimum-purchase thresholds and a 20% retroactive late-renewal penalty raise both cost and rigidity — and Broadcom has already tested tightening these further once
- Broadcom is also narrowing its reseller/cloud-partner ecosystem — a risk if ACS's current VMware support relationship sits with a partner not re-invited into the new program
- **Net effect on ACS:** higher, less flexible licensing cost + reduced negotiating leverage + potential channel/support continuity risk

**Speaker note / flag (not on-slide):** ⚠️ **Time-sensitive — re-verify before the board meeting.** The specific core-minimum thresholds, current bundle SKU pricing, and VCSP partner-program dates (legacy program closed, contracts not renewing past **Jan 26, 2026**, transact-only window to **Mar 31, 2026**) are moving targets Broadcom has changed multiple times since 2024. Confirm current figures against Broadcom's partner portal and ACS's account rep before finalizing this slide. Do not present exact dates/numbers as static facts without that check.

---

## Slide 3 — The Alternative Landscape

**Layout type:** Comparison table slide

**Purpose / one-line takeaway:** A handful of credible, proven alternatives exist — the board doesn't need to evaluate all of them in depth, just recognize the shape of the market.

**Content:** Condensed comparison table, 6 rows × 3 columns (trim the brief's 4-column table to fit one board-legible screen — drop the "headline trade-off" prose column into a shorter phrase, or split trade-off into a compact tag). Suggested compression:

| Option | Best fit for ACS if… | One-word trade-off |
|---|---|---|
| **Nutanix (AHV)** | Large estate (200+ VMs), wants an integrated like-for-like replacement | Premium cost, new lock-in |
| **Microsoft Hyper-V / Azure Local** | Already deep in Microsoft stack, smaller estate (<50 VMs) | Weak fit for Linux/mixed |
| **Proxmox VE** | Mid-size (50-200 VMs), cost-conscious, hands-on team | Smaller support ecosystem |
| **Red Hat OpenShift Virtualization** | Already on/planning Kubernetes | Steep learning curve |
| **Citrix Hypervisor / XCP-ng** | Existing Xen shop, wants open-source + commercial backing | Smaller tooling ecosystem |
| **Public-cloud re-platforming** | Specific workloads better off re-architected, not lifted | Modernization project, not a swap |

**Design note:** if 6 rows reads too dense on the ACS content master, cut to the 3-4 most relevant rows for ACS's actual estate profile (Nutanix, one open-source option, Hyper-V) and mention the rest verbally — table density ceiling is 4-7 rows per Charta's own layout heuristics, 6 is at the edge and only works if row text stays this short.

---

## Slide 4 — How We'll Evaluate Any Shortlist

**Layout type:** Bullet content slide (5 items — consider a simple icon-per-axis feature-grid treatment if the ACS content master supports icon bullets; otherwise plain 5-bullet list)

**Purpose / one-line takeaway:** Any deeper vendor comparison will be scored against these five dimensions, so the board knows what "rigorous evaluation" means before authorizing next steps.

**Content:**
1. **Total cost of ownership (3-5 yr)** — license/subscription + migration + retraining, benchmarked against the cost of *not* moving
2. **Migration risk and effort** — how much of the estate moves, how disruptive the cutover is, realistic timeline (large migrations commonly run 6-24 months)
3. **Operational maturity fit** — does ACS's team already have the skills the alternative demands, or is re-skilling investment required
4. **Vendor lock-in / strategic independence** — is the new dependency better-positioned than the current one
5. **Support and ecosystem maturity** — enterprise support depth, third-party tooling, channel-partner availability

---

## Slide 5 — Recommended Next Step

**Layout type:** Bullet content slide (or closing-adjacent "decision" layout if the ACS master has one — otherwise standard content layout)

**Purpose / one-line takeaway:** This is not a vendor decision today — it's a request to authorize a shortlist-and-RFP process, with an optional low-risk pilot in parallel.

**Content:**
- **Shortlist 2-3 candidates** from the landscape (likely Nutanix + one open-source option + Hyper-V, depending on ACS's estate profile)
- **Route the shortlist to Marlowe** for formal TCO/RFP evaluation against the five axes on the prior slide
- **Consider a non-critical pilot** (single workload cluster or DR/secondary environment) in parallel, to de-risk migration-effort unknowns before committing the primary estate
- **Decision timing** should be set by ACS's actual VMware renewal date and current partner/support status — to be confirmed and layered in before a target decision date is set
- **What we're asking the board for today:** approval to proceed with the shortlist + RFP process (not a vendor selection)

**Speaker note / flag (not on-slide):** Final vendor selection is explicitly Egon's call once RFP work completes — this slide asks for process authorization only, not a vendor endorsement. Keep that framing verbal if not already implied by the "what we're asking for" bullet.

---

## Slide 6 — Closing / Questions (optional)

**Layout type:** Closing slide (ACS template closing master)

**Purpose / one-line takeaway:** Standard close — signal the presentation is done and open the floor, per normal ACS board-deck convention.

**Content:**
- "Questions & Discussion" (or ACS's standard closing-slide phrasing, if the template has fixed boilerplate text — check the master before overriding it)
- Optional: presenter contact / follow-up owner (Egon, Ansel for ecosystem-watch questions, Marlowe once RFP is authorized)

---

## Time-sensitive figures — re-verify before the board meeting

Flagging these explicitly per Ansel's own brief caveat, so whoever presents checks before finalizing slide 2:

1. **Core-minimum purchase thresholds** — currently 16-core-per-CPU minimum; Broadcom floated (then retracted) a 72-core minimum in April 2025. Confirm current threshold.
2. **Bundle SKU pricing / current packaging** — VMware Cloud Foundation pricing and bundle structure have shifted multiple times since 2024. Confirm current pricing against Broadcom's partner portal.
3. **VCSP partner-program dates** — legacy program closed; non-renewal beyond **January 26, 2026**; transact-only close-out window to **March 31, 2026**. Confirm these dates haven't shifted again and confirm whether ACS's own support/resale relationship runs through an affected partner.
4. **ACS's own VMware renewal date and current partner/support relationship status** — not yet confirmed anywhere in the brief; this is what should actually set the board's urgency/timeline framing, and it's an open dependency Ansel flagged, not a settled fact.

None of the above should appear on slide 2 as static, unqualified figures without a same-week check — Broadcom has changed these terms multiple times since 2024 and may again before the board meets.

---

## Deferred / out of scope for this deck

- Vendor-by-vendor TCO/RFP comparison — belongs to Marlowe, post-shortlist-authorization, not this board briefing.
- ACS-specific contract terms, negotiated pricing, or partner-tier standing — per [[GL-006-confidential-vendor-data-handling]], these stay in controlled storage and are out of scope for a board deck built from public-market sourcing.
- Final vendor selection / migrate-or-stay call — Egon's decision once RFP work is complete, not represented as a decision point in this deck.

## References

- [[2026-07-01-broadcom-vmware-alternatives-brief]] — source content, written by Ansel.
- [[GL-008-acs-branding-templates]] — template selection rule; this deck uses `Slide presentazione ACS_2026.potm`.
- [[GL-003-design-system]] — house design system; explicitly not used for this ACS deliverable (GL-008 overrides).
- [[SOP-010-vendor-evaluation-and-rfp-process]] — the process the shortlist routes into after this board briefing (Marlowe's territory, referenced on slide 5, not executed here).
