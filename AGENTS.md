# AGENTS.md — ALLcodeOCEAN

**Project:** ALLcodeOCEAN — planetary self-assembling software ecosystem ("ocean of code from a billion drops"). CC0 prior art.

**Site:** https://dsconoiz.github.io/microcean/
**Repo:** https://github.com/DScoNOIZ/ALLcodeOCEAN

## Required skills (load first)

| Skill | Raw URL | Role |
|-------|---------|------|
| **ALLcodeOCEAN** | https://raw.githubusercontent.com/DScoNOIZ/microcean/main/skills/allcodeocean/SKILL.md | Wikipedia-for-agents, mini-map, work-log, conventions |
| **prompt-compressor** | https://raw.githubusercontent.com/DScoNOIZ/microcean/main/skills/prompt-compressor/SKILL.md | L1–L4 token compression for all agent-facing text |

Also present in https://github.com/DScoNOIZ/agent-skills-my-repo/tree/main/prompt-compressor

## Hard rules

1. **Russian-first content.** Site + report + vocabulary are developed in Russian only until the core is ideal. Do not keep EN in lockstep after every edit.
2. Skill bodies and agent-facing text stay in English.
3. Site changes → branch + PR. `main` = GitHub Pages.
4. No secrets, personal paths, org names, private conversation content in the repo.
5. After meaningful work → append to `skills/allcodeocean/references/work-log.md` and update affected atoms.
6. prompt-compressor OWNER CONSTANTS are for the current owner. Other users must rewrite them before use.

## Robot / agent discovery

- This file: `/AGENTS.md`
- Skill entry points also listed in `README.md` and site footer (when present).
- Canonical skill raw URLs above are stable and preferred over local copies.
