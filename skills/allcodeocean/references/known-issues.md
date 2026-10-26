# Known issues (findings from the 2026-10-26 review). Status key: PREPARED = fix written and validated on a separate branch, awaiting maintainer approval (not yet in the repo); OPEN-DECISION = author's call; OPEN = needs work.

## A. Unambiguous defects
| ID | Issue | Status |
|---|---|---|
| A1 | `ru/glossary.html`: `<dt>…</td>` (Amdahl) and `<td>` used instead of `<dd>` (Compromise) | PREPARED |
| A2 | `ru/limits.html` lines ~83-86: `<li>…</td>` | PREPARED |
| A3 | RU glossary typos: "клиентовwelcome", "Риissanена", "Пропускная способность / Пропускная способность (Throughput)" | PREPARED |
| A4 | Duplicate RU glossary entry "Колмогоровская сложность K(x)" (kept the version with citations) | PREPARED |
| A5 | Leaked internal line on scientist pages: "Справочно (факт-чек публикации): пакетов 50,5% / зависимостей 50,6%; ASCII-диапазоны токенов — 25,000-50,000 / 96-97% / 60-80% / 200-500 / ~80%." Added in commit 7575021 ("add missing numbers"); no other page or ledger entry references these numbers. Removed in RU and EN | PREPARED |
| A6 | Calque "Торрент-фо-код" → "Торрент для кода" (RU), "Torrent-for-code" → "A torrent for code" (EN) | PREPARED |
| A7 | Nonsense word "нашихвов" in the harmony slogan → "швов" (guess; EN mirror says "stitches") | PREPARED (flag the guess) |
| A8 | Same sentence repeated twice on one page (philosophy RU/EN) | PREPARED |
| A9 | RU glossary 44 terms vs EN 49 | OPEN |
| A10 | Private file-system path in one ledger line of `OTCHETY/REPORT.md`: removed from the working tree on 2026-10-26. Git history still contains the old text (harmless local directory/user name; rewriting history is not recommended). Organization-name and private-wiki-path references remain in a few `OTCHETY/` files and in the two-date-chain sentence on the pages | PARTLY FIXED; remaining items OPEN-DECISION |

## B. Content/logic problems (not changed; author's decision)
| ID | Issue |
|---|---|
| B1 | E2 headline compares 2·10^4 evals to 10^101 although the experiment space is 10^20 and fitness is separable (see evidence file) |
| B2 | E10 and E3 results are built into the model; used on the home page as evidence |
| B3 | "Proven" labels attach to theorems/model simulations, not to the system |
| B4 | Glossary says "no energy-hungry PoW / trust without blockchain" while limits.html proposes "PoW/PoS at entry", stakes, slashing, queue-of-rights ("law in code") |
| B5 | Reputation by executable tests contradicts the site's own Rice's-theorem point; tests are authored by the fragment's author (adversary); xz backdoor hid in test files and used years of social engineering |
| B6 | "No monoculture" vs selection/preferential attachment; popular fragments win everywhere (Log4Shell pattern). Micro-granularity increases author count and trust decisions (left-pad was a micro-package; its cause was npm unpublish policy) |
| B7 | DHT gives exact-key lookup; "find fragments by class/meaning" needs a semantic index; 5.4 hops is not latency |
| B8 | Spec problem: natural-language goal → executable spec is hand-waved ("top layer model"); composition ∘ and a common IR/type system undefined; glue code ignored (assembly is a graph, not a subset) |
| B9 | Centralization remains: top-layer model operator, PBFT coordinator council (PBFT needs known membership, O(n²) messages), lagoons recreate an archipelago |
| B10 | Gossip-pushed updates/revocations are themselves an attack channel (SolarWinds-style auto-update, false revocations) |
| B11 | Citation-graph reputation is gameable (link farms); stake excludes hobbyists and needs an oracle for "maliciousness" |
| B12 | Program ≠ code: payments, notifications, hosting, accounts, compliance are not fragments; scenario times ("minutes") unsubstantiated |
| B13 | Literature claim: "100+ works", but the list has 47 items (1-40 external theory/mechanism sources, 41-47 internal working materials); sources include Wikipedia/GeeksforGeeks/blogs; no software-ecosystem analogues cited (see analogues.md). "Origin of materials" section does not say whether AI/agent tools were used (the repo contains an agent report board and role labels such as "Исполнитель: data_analyst") |
| B14 | License compatibility of auto-assembled fragments (GPL/AGPL/MIT/proprietary) unaddressed; CC0 on the concept text does not license fragments |
| B15 | Evolutionary core vs LLM synthesis: on benchmark studies Copilot beat GP (reported 85.2% vs 77.8% solved), and a 2025 PushGP vs GPT-4o comparison found no clear winner; the site does not argue why assembly beats on-the-fly generation |

## C. Intentionally left as is
- The "harmony" slogan ("Гармония: атомы, не кирпичи…") on index/uchenym/etc.: inserted deliberately in commit e7f8678 ("per operator articulation (constraints preserved)"). A first review pass wanted to remove it everywhere; after tracing history it was kept. Only the exact in-page duplicate was removed. Tone mismatch in disclaimer/science paragraphs is a suggestion, not a defect.
