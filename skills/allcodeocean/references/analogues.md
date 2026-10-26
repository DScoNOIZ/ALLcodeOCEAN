# Analogues and counter-evidence (found 2026-10-26; re-verify before quoting)

| Item | Why relevant | Link |
|---|---|---|
| Joe Armstrong, "Why do we need modules at all?" (erlang-questions, 2011) | Proposal for one global database of functions with metadata, content hashes, no separate projects — near-identical early form of the idea | https://erlang.org/pipermail/erlang-questions/2011-May/058768.html |
| Unison language | Code addressed by hash of the syntax tree, distributed functions, immutable definitions; 1.0 reported Nov 2025 | https://www.infoworld.com/article/4100673/futuristic-unison-functional-language-debuts.html |
| Radicle | Peer-to-peer code collaboration on Git with gossip and CRDT-based objects | https://lwn.net/Articles/966869 |
| Nix + IPFS | Content-addressed derivations/sources on a P2P store | https://blog.obsidian.systems/nix-x-ipfs-milestone-1/ |
| Guix + Software Heritage | Universal archive of source code as substrate for reproducible builds | https://www.arxiv.org/pdf/2405.15516 |
| Trivial-package studies (npm) | Micro-package risks: many have deps, few have tests | https://neverworkintheory.org/2021/09/17/why-do-developers-use-trivial-packages.html |
| GP vs LLM program synthesis | Evolutionary core vs LLM generation | https://gpbib.cs.ucl.ac.uk/gp-html/Sobania_ieeeTEC2.html ; arXiv 2508.03966 |
| Kademlia/Mainline DHT measurements and attacks | Real-world latency, Sybil/eclipse | https://www.cl.cam.ac.uk/~lw525/MLDHT/ ; https://ix.cs.uoregon.edu/~lijun/pubs/pdfs/liu12kad.pdf ; https://www-users.cs.umn.edu/~hopper/kad_attack_journal.pdf |
| xz backdoor (CVE-2024-3094) | Social-engineering supply-chain attack hidden in test artifacts; tests do not catch it | https://arxiv.org/html/2404.08987v1 ; https://strobes.co/research/xz-utils-backdoor-supply-chain-attack-dissected |

Also relevant but not researched in depth: WebAssembly component model/registries (common IR + typed interfaces), CEGIS/SyGuS literature, Hackage/Hoogle-style type search, Software Heritage scale.
Effort note: about 60 external pages were consulted in the first review; broaden the source base before making strong claims.
