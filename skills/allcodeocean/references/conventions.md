# Conventions and operator directives

## Language policy (authoritative, 2026-10-26)

**Russian-first development.**

- Primary language of all content work is **Russian**.
- The Russian version is the single source of truth until it is considered ideal and stable.
- Do **not** maintain parallel EN (or other language) versions in lockstep after every edit.
- Synchronizing multiple languages after every small change is rejected as unrealistic and wasteful.
- Translation to English and other languages is deferred until the Russian core is polished.
- This policy is deliberate: one perfect version first → then translation. Avoid doing the same work N times.

When the Russian core is ready for translation, this section will be updated.

## Other standing rules

- **Impersonal public voice**: no first-person private infrastructure, paths, organization names or codenames on public surfaces.
- **Honesty markers**: evidence labels [ДОКАЗАНО]/[ПРАВДОПОДОБНО]/[НЕВОЗМОЖНО]; estimates are hedged; a limits page exists. Do not strengthen claims.
- **Fact-check discipline**: numbers are traced in `OTCHETY/FACTCHECK-LEDGER.md`. If you change a number, update the ledger/report. (Language policy above applies.)
- **Board etiquette**: record intent before editing site prose; one line per action in logs; never rewrite past entries.
- **Commit style**: `type(scope): summary` (feat/fix/docs; scopes content, legal, privacy, factcheck, site, i18n, board).
- **Static site**: no build, no JS deps; keep CSS in `assets/style.css`; validate tag balance and links after edits.
- Slogan/metaphor language ("ocean", "plankton", "lagoons", "harmony") is the operator's articulation; edit with care.
- Show verification (validation output, diffs of removed text), not just claims.

## Skill-specific rules

- This skill is the shared Wikipedia-for-agents (mini-map + navigator + progress log).
- Keep it atomic and fully interlinked.
- Always write skill content itself in **English** (this is the agent-facing layer).
- After any meaningful repo change, transfer the essence into the skill: what was done, why, how, and the reasons for the edit. Append to `work-log.md` and update affected atoms.
