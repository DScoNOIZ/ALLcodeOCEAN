# Proposed improvements (reviewer proposal, not decisions)

1. **Reframe the thesis**: a content-addressed registry of typed, capability-declared code units plus agent-assisted assembly. Make "micro" optional (the site already allows any granularity).
2. **Stand on existing work**: hash-addressing (Unison), reproducible builds (Nix/Guix), corpus (Software Heritage), P2P layer (Radicle/IPFS), common IR with typed interfaces (WebAssembly component model). Add an analogues page and credit Armstrong 2011.
3. **Assembly core**: LLM proposes, deterministic verifier decides (types, property tests, sandbox); evolutionary search only for resource optimization. Benchmark against plain LLM generation on real tasks (size, bugs, vulnerabilities).
4. **Security**: capability-based isolation (a fragment can do only what it declares), signed provenance, independent auditor attestations instead of author tests, pinned hashes with staged rollout instead of auto-push updates, transparency log.
5. **Trust without tokens**: reputation of independent verifiers, public logs; resolve the PoW/stake contradiction explicitly.
6. **Spec layer**: define how a human goal becomes an executable spec and what ∘ means; model assembly as a graph with glue.
7. **Experiments**: binary/rugged fitness, real code, interacting fragments, preregistered, negative results published; stop labelling model simulations "proven".
8. **Legal**: license-compatibility engine, provenance, trademark check, accurate prior-art language, real timestamps (OpenTimestamps/DOI).
9. **Editorial**: remove duplicates/leaks, disclose AI involvement, fix RU/EN glossary parity, align the "100+" claim with the list.
10. **Narrow prototype first**: one language, curated corpus, measured against baselines.

## Skill-as-Wikipedia improvements (2026-10-26)

- [x] Sync full local skill atoms to repo (policy + checklist pushed 2026-10-26)
- [ ] Add short "status of each atom" table in SKILL.md (fresh / stale / needs review)
- [ ] Cross-link every atom to work-log entries that last touched it
- [x] Add "How to contribute as an agent" checklist to SKILL.md
- [ ] Ensure every known-issue has a status + owner + next action
- [ ] Add machine-readable frontmatter keys for last-verified date and policy version
