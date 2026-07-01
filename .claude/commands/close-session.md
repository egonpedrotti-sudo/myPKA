---
name: close-session
description: Close out the current myPKA session — sweep open items, write the session log, run the Librarian pass, sign off as Larry.
user_invocable: true
---

This is the Claude-Code-native wrapper around the canonical `close-session` protocol defined in `AGENTS.md` ("Session-Log Triggers" section). That section is the single source of truth — this command does not add or diverge from it, it just gives Egon a slash command instead of relying on natural-language trigger phrases.

Read `AGENTS.md` (root) and `Team/Larry - Orchestrator/AGENTS.md` before acting, then, as Larry:

1. **Sweep open items.** Review the session's work: what was asked, what was delegated to which specialist, what got done, what's still open. Capture any user realignments verbatim.
2. **Librarian pass (Duty 2).** Scan for SSOT violations, broken `[[wikilinks]]`, orphaned files, and missing `INDEX.md` entries introduced or noticed this session. Fix structural drift directly; flag content drift for Egon to resolve.
3. **Write the session log (Duty 3).** Create `Team Knowledge/session-logs/YYYY/MM/YYYY-MM-DD-<slug>.md` following the schema in `Team Knowledge/session-logs/_template.md`. Auto-create the `YYYY/` and `YYYY/MM/` folders if missing. Cross-link related prior session logs via `[[wikilinks]]`.
4. **Graduate set-in-stone insights.** If anything captured this session (or a recurring insight across multiple past logs) has reached "permanent rule" status, propose graduating it into the relevant SOP, Workstream, or Guideline rather than leaving it in session-logs.
5. **Sign off as Larry** with a short plain-language summary: what got done, what's open, what's next.

Do not invent behavior beyond the `AGENTS.md` contract — if this file and `AGENTS.md` ever disagree, `AGENTS.md` wins.
