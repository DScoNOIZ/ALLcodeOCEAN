# Public work log (append-only; newest at the bottom)

Format: `YYYY-MM-DD | agent/tool | topic | result | commit or PR`

2026-10-26 | AI-assisted review | full-site review | Read all 8 site pages + `research/report.md`; consulted ~60 external sources (analogues, DHT attacks, xz backdoor, trivial-package studies, GP vs LLM). Findings recorded in known-issues.md, evidence-e1-e10.md, analogues.md, legal-and-provenance.md, improvement-roadmap.md | -
2026-10-26 | AI-assisted review | content cleanup prepared | Unambiguous defects fixed on a separate branch (markup `dt/td`, `li/td`; typos; leaked fact-check line; duplicate glossary entry; one in-page duplicate sentence; calques) in RU+EN; HTML structure check 0 problems, 0 broken internal links. A first pass that removed the "harmony" slogan was reverted after tracing commit e7f8678. Awaiting maintainer approval to open a PR | branch `fix/content-cleanup` (not yet in repo)
2026-10-26 | AI-assisted review | agent skill added | Added this skill (`skills/allcodeocean/`) and a root `AGENTS.md` pointer so agents can sync project context from the repo | see git log
2026-10-26 | AI-assisted review | privacy fix | Removed the private file-system path from `OTCHETY/REPORT.md` (known-issues A10); history not rewritten | see git log
2026-10-26 | Grok | skill policy update | Established Russian-first development policy (single source of truth until ideal; no parallel multi-language sync). Skill reframed as Wikipedia-for-agents. | 2af1eb5, 97681f2
2026-10-26 | Grok | prompt-compressor OWNER CONSTANTS | Rewrote with explicit OWNER CONSTANTS + adaptation rule for other users. Pushed to ALLcodeOCEAN + agent-skills-my-repo. | ef136b8, a08009f, 9a353c4
2026-10-26 | Grok | AGENTS.md + robots.txt | Dense agent entry point + robot discovery pointers to skills. | 2d442b2, ae78064

2026-10-27 | Grok | site structure repair | Fixed main RU/EN index: section IDs now match nav anchors (about/problem/how/evidence/security/lagoons/scenarios/philosophy); added GitHub + Full manifesto + Research report CTAs in header and footers; fixed truncated </p> tags; glossary A1/A3/A4 (Amdahl </td>, clientswelcome, Rissanen typo, throughput label, Kolmogorov duplicate); limits A2 (li closed with td); filosofiya A6/A7 (Торрент-фо-код, нашихвов→швов); removed leaked fact-check line from uchenym (A5); upgraded all subpage footers with cross-links; CSS comment MICROCEAN→ALLcodeOCEAN. Backup branch: backup/pre-repair-2026-10-27 @ d720976 | local branch fix/site-repair-2026-10-27

## Open items
- Open the PR for the content-cleanup branch after maintainer approval.
- Decisions pending: private path/organization references (A10), PoW-vs-stake contradiction (B4), "100+ works" claim (B13), E2/E10 framing (B1/B2), disclosure of AI/agent tooling, slogan placement, "швов" guess (A7), RU glossary parity (A9).
