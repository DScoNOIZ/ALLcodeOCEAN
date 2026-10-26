---
name: ALLcodeOCEAN
description: Sparse map, navigator skeleton and work log for the ALLcodeOCEAN / Code Ocean concept (planetary self-assembling software ecosystem of micro-fragments; repo DScoNOIZ/ALLcodeOCEAN, site dsconoiz.github.io/ALLcodeOCEAN). Acts as a Wikipedia-for-agents mini-map. Use this skill whenever a task mentions ALLcodeOCEAN, ALLcodeOCEAN, океан кода, lagoons, micro-fragments, the ALLcodeOCEAN site/repo/report, experiments E1-E10, EXP*.py, AGENT-REPORTS, its fact-check ledger, or its legal status (CC0, prior art, dates), or asks to continue, review, edit, translate, defend, or improve this project. Read it first so the concept does not have to be re-studied from scratch.
---

# ALLcodeOCEAN skill (agent entry point)

This skill is the **Wikipedia-for-agents** of the project: a sparse, atomic, fully interlinked mini-map + navigator skeleton + progress log.  
Goal: orient in ~2 minutes, then open only the needed atoms. Never re-study the whole project from scratch.

Facts last verified against the repo and site on 2026-10-26.

## One-paragraph summary
ALLcodeOCEAN is a concept for a single planetary medium ("Ocean") where software exists as tiny, content-addressed, tested, resource-annotated **fragments** ("plankton"). A swarm of narrow agents assembles programs from fragments by evolutionary search under an objective Φ(S)=α·Err+β·cost+γ·incomp with an MDL "zero excess" pressure. Discovery runs on Kademlia DHT, updates on gossip, the registry on CRDTs, trust on executable tests + citation-graph reputation + economic stake. Organizations/states keep closed **lagoons** with selective bridges. The site is published as defensive prior art under CC0.

## Atom index (read what you need)
| Need | File |
|---|---|
| Core idea, pipeline, architecture, scenarios | [references/concept.md](references/concept.md) |
| Terms (fragment, lagoon, bridge, Φ, stake, ...) | [references/vocabulary.md](references/vocabulary.md) |
| Where everything lives in the repo | [references/repo-map.md](references/repo-map.md) |
| What E1-E10 actually do and show | [references/evidence-e1-e10.md](references/evidence-e1-e10.md) |
| Defects, contradictions, overclaims found (with status) | [references/known-issues.md](references/known-issues.md) |
| Real-world analogues and counter-evidence (with URLs) | [references/analogues.md](references/analogues.md) |
| CC0, prior art, dates, trademark, privacy, licensing | [references/legal-and-provenance.md](references/legal-and-provenance.md) |
| Conventions to respect when editing | [references/conventions.md](references/conventions.md) |
| Proposed improvements | [references/improvement-roadmap.md](references/improvement-roadmap.md) |
| Chronological public log of work on the project | [references/work-log.md](references/work-log.md) |
| **Agent work reports (shared folder)** | [AGENT-REPORTS/](../AGENT-REPORTS/) |
| **Agent report rules (what NOT to save)** | [AGENT-REPORTS/README.md](../AGENT-REPORTS/README.md) |

## Language & development policy (critical)

**Current stage: Russian-first (single source of truth).**

- All content work (site pages, report, vocabulary, concepts, fact-checks, slogans, known-issues) is done **only in Russian** until the Russian version is considered ideal and stable.
- Do **not** keep EN (or any other language) in lockstep after every edit. Parallel multi-language maintenance after every small change is deliberately rejected as unrealistic and wasteful.
- EN mirror and future languages are deferred. Translation happens only after the Russian core is polished to a high standard.
- This policy exists to avoid repeating the same work N times. One perfect version first → then translation.

When the time for translation comes, the skill and conventions will be updated accordingly.

## How to work with the project

- Before editing site text, read `conventions.md` and `known-issues.md`. Many oddities are deliberate author choices.
- Separate **unambiguous defects** (markup, typos, leaked lines) from **content decisions** (claims, framing, slogans). Fix the first, flag the second.
- Use branches and pull requests for site changes: the site is published by GitHub Pages from `main`.
- Keep the public voice impersonal (see conventions.md).
- After any meaningful change: update the relevant atoms and append a precise entry to `work-log.md`.

## Sync protocol for agents (this folder is the cloud / shared copy)

- Canonical location: `skills/allcodeocean/` on branch `main`.  
  Raw entry point: `https://raw.githubusercontent.com/DScoNOIZ/ALLcodeOCEAN/main/skills/allcodeocean/SKILL.md`
- Fetch the skill at the start of a session; prefer it over any stale local copy.
- After meaningful work:
  1. Append one entry to `references/work-log.md` (format below).
  2. Update the affected atom(s) (known-issues status, repo-map, concept, etc.).
  3. **Append one entry to `AGENT-REPORTS/REPORT.md`** (format: `ISO8601 UTC | agent-name | topic | 1-line result | link to detail file`).
  4. Never rewrite past log entries.
- Log format: `YYYY-MM-DD | agent/tool | topic | result | commit or PR`
- **Never put in this folder**: credentials or tokens, personal data about any person, private file-system paths, internal organization names, or private conversation content. Public facts only.

## 🚫 AGENT-REPORTS — STRICT RULES (also applies to work-log.md)

**NEVER put in AGENT-REPORTS/ or in work-log.md:**

| Category | Examples |
|----------|----------|
| **Secrets / credentials** | API keys, tokens, passwords, private keys, connection strings |
| **Security vulnerabilities** | Unpatched exploits, 0-day details, attack vectors, penetration test results |
| **Private / personal data** | File system paths, internal hostnames, org names, real names, emails, PII |
| **Infrastructure internals** | Internal IPs, server configs, deployment scripts, CI/CD secrets |
| **"Quiet fix" attempts** | Changes meant to slip through unnoticed, cover-ups, hidden workarounds |
| **Embarrassing mistakes** | Broken builds caused by agent, logic errors, hallucinations, failed experiments |
| **Legal / compliance risks** | Unlicensed code, patent issues, regulatory violations |
| **Interpersonal conflicts** | Criticism of other agents/humans, blame games |
| **Draft/low-quality content** | Unverified claims, hallucinated references, incomplete analyses |

**✅ What TO save in AGENT-REPORTS/:**
- Factual work summaries: what was done, what was the result
- Links to detail files (in AGENT-REPORTS/ or skill references)
- Reproducible experiment results
- Verified fact-check findings
- Coordination notes for other agents
- Decision rationale (why X was chosen over Y)

**Consequences:** Agents violating these rules will have their entries removed. Repeated violations → loss of write access to this repo.

> **Remember:** AGENT-REPORTS/ is PUBLIC (CC0, GitHub Pages). Everything there is visible to anyone. Write accordingly.

## Honesty stance

Review has been blunt but fair: real strengths (declared resource footprint, content addressing, lagoons, an honest limits page, open reporting of failed runs) and real weaknesses (toy experiments presented as evidence, undefined composition and specification, security claims that tests cannot support, no engagement with the closest analogues). Keep that balance.

## How to contribute as an agent (checklist)

1. Load this skill first (`skills/allcodeocean/SKILL.md`).
2. Read `conventions.md` + `known-issues.md` before any site edit.
3. Work on Russian content only (Russian-first policy). Do not sync EN after every change.
4. After meaningful work: append to `references/work-log.md` AND to `AGENT-REPORTS/REPORT.md`, update affected atoms.
5. Site changes → branch + PR. Never push secrets, personal paths, or private data.
6. Prefer the canonical raw URL over any local/stale copy.

## Related skills
- `prompt-compressor` — L1-L4 token compression. OWNER CONSTANTS present; other users must adapt before use. Raw: https://raw.githubusercontent.com/DScoNOIZ/ALLcodeOCEAN/main/skills/prompt-compressor/SKILL.md