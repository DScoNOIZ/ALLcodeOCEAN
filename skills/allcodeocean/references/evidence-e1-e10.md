# What E1-E10 are (from research/report.md §0, verified numbers)

Labels used by the site: [ДОКАЗАНО] proven, [ПРАВДОПОДОБНО] plausible, [НЕВОЗМОЖНО] impossible, [ОБЩЕИЗВЕСТНО] known.

| # | Setup | Reported result | Review note (see known-issues.md) |
|---|---|---|---|
| E1 | C(10^6,20) subsets | ≈10^101.61; GA "sees" ≈10^-97 | Brute force is a strawman; real assembly is a wired graph, not a subset |
| E2 | GA, L=20 slots, M=10 options | 30/30 success for N=50/100/200; first hit at gen 38.7/25.3/20.6 | Actual space 10^20, fitness = fraction of slots matching a known target (separable, OneMax-like). Headline "2·10^4 evals instead of 10^101" compares different spaces; ~200 evals suffice if slots are independent. The ~2·10^4 is the budget N·G; first hit at N=100 is ~2,500 evals |
| E3 | Epistasis λ | λ=0,0.3 → correlation 1.0; λ=0.7 → 0.325±0.109; λ=1.0 → 0.178±0.068 | Conflict term is constructed against the target; failure is by design; useful only as a qualitative warning |
| E4 | GDC sizing | N_s=2cκσ²/d²; at σ_M/d=4: 173.19 (c=z²≈2.71, κ=2); empirical N*=50-100 (factor 1.7-3.5) | Theory fits the assumed noise model, not software; fact-check unified c (was split-brain 196 vs 125.44) |
| E5 | Kademlia model, b=64, k=20, 1000 lookups/network, seed 42 | n=10^9: 5.42±0.83 hops (max 8); ceil log2 n = 30 | Generative model, not a live network; hops ≠ latency; no churn/Sybil/eclipse; DHT is exact-key lookup, not semantic search |
| E6 | Gossip push-pull (Karp 2000) | n=10^5: 11.37±0.48 rounds vs log3 n=10.48 (ratio 1.08) | Complete graph, no loss/async |
| E7 | CRDT monoid laws | 10000/10000 law checks; replicas 1000/1000 | Counters/sets only; code trees are harder |
| E8 | Amdahl | p=0.99: S(1024)=91.2, S(∞)=100; p=0.95: 19.6→20 | Formula evaluation with arbitrary p, not an experiment |
| E9 | CEGIS toy | synthesizes max(x,y)=ite(x<y,y,x); 1 iteration, 820 candidates; impossible without `<` | Framework demo only; no scaling evidence |
| E10 | MDL "zero excess" | zlib on duplicates 159→265 B while raw 200→18600; MDL-GA length 150.9→60.9 at correctness 1.0 (2.5× shorter); r(raw,correct)=−0.91, r(zlib,correct)≈0 | Short/long correct variants are built in; correlation "by construction" per the report; circular as evidence |

Reproduction facts: run 2026-10-26 (Python 3.14.7, numpy 2.5.2); 9/10 totals matched, EXP6/EXP8 matplotlib-dependent; FC-C found one false claim (E4 GDC split-brain, fixed).
Honest features worth keeping: failed first E6 run disclosed; repro verdicts stated; limits page.
