# Concept (condensed from the site, EN mirror, research/report.md)

## Thesis
All software of the planet as one continuous medium ("one water"), not an archipelago of repos/packages/IDEs/CI. Basic reuse unit = a fragment of exactly the needed size ("zero excess"). Code, history and practice are neighboring regions of one sea.

## Pipeline (site section "How the system is arranged")
1. A person states a goal in plain language; a high-level model (top layer) turns it into a spec/task decomposition.
2. Discovery: DHT lookups find fragments by class; fragments carry interface, pre/post-conditions, hash, semantic tags, reputation, measured resource profile.
3. Assembly: a **swarm** of narrow agents (neural and algorithmic) proposes assemblies; evolutionary search minimizes Φ(S)=α·Err(S,Spec)+β·cost(p(S))+γ·incomp(S), α≫β,γ; cost = full resource footprint (size, time, memory, traffic, energy). MDL gives the size penalty.
4. Verification: executable tests (+ bounded-property checks, CEGIS ideas); results feed reputation.
5. Distribution: fragment updates by gossip push-pull; registry and "queue-of-rights" as CRDTs (ORSet for multi-author); consensus only where needed (Raft inside a trusted cluster; PBFT for a coordinator council; hashgraph mentioned).
6. Resource honesty: the client declares the footprint (downloads, compute, energy) and asks consent before installing.

## Granularity ladder (no rigid levels)
plankton (micro-fragments) → schools of fish (functions/modules) → islands (packages/apps) → ecosystems (stacks). Libraries are "whales and reefs": used whole when mature.

## Lagoons and bridges
Closed circuits for organizations/states with their own fragments and history; **bridges** import/export selectively under owner rules. Lagoon trade-off: "zero leaks" but poorer without inflow.

## Security story as claimed
No monoculture; compromise of one fragment is local; threat info spreads by gossip; Sybil resistance via stake at entry + reputation on the citation graph (not on nodes); garbage-flood mitigation via stake and MDL pressure. See known-issues.md for why several of these are weak.

## Scenarios on the site
Everyday person ("reminder for mom", small game), engineer, scientist, organization lagoon. Time-to-result figures are labelled design estimates, not measurements.

## Three exposition levels
For everyone (`ru/vsem`), specialists (`ru/specialistam`), scientists (`ru/uchenym`: formal model, E1-E10), plus philosophy, limits, glossary.

## Honest limits stated by the site itself
No universal builder for "any program" (No Free Lunch), no absolute minimality (K(x) uncomputable), parallelism capped (Amdahl), no convergence guarantee (schema theorem is expectation only), no Sybil immunity without economic stakes, no legal invulnerability, no immunity to fragment garbage without stakes/MDL pressure.
