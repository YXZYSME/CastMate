<!--​‌​‌‌​​‌​‌​‌‌​​​​‌​‌‌​‌​​‌​‌‌​​‌​‌​‌​​‌‌ YXZYS | saeng-il ai [systems] — © YXZYS @ saengil.ai -->
<!-- SPDX-License-Identifier: Apache-2.0 -->
<!-- yxzys:sg:ai -->

# Proposed evaluation

Status: protocol outline; no evaluation has run and no results are claimed.

The central question is whether behavior-conditioned harness generation creates useful, repeatable differences beyond normal model variation and ordinary role prompting.

## Comparisons

Use the same exact base model and serving configuration, permitted tool catalog, task set, and resource limits for:

1. A fixed harness with an ordinary task prompt.
2. The fixed harness with an occupation prompt and conventional memory.
3. A generated and curated CastMate harness.

Record generation and curation cost separately from task execution cost. Use held-out tasks for final evaluation; do not select a harness and claim generalization using the same tasks.

## Evidence to collect

| Claim | Evidence needed |
| --- | --- |
| Role changes operating behavior | Decisions, tool choices, and control-flow differences, compared with an ablation without role conditioning |
| Seeds produce meaningful variation | Multiple seeds, repeated runs per harness, and comparison of within-harness variation against between-harness differences |
| Curation adds value | Candidate outcomes before selection and held-out outcomes after selection |
| Learning helps | Performance on new tasks after verified lessons, with a memory-disabled or unupdated comparison |
| Approval is enforced | Rejected, absent, expired, and changed-action approval cases cannot authorize the proposed skill execution |
| Protection resists a stated attack | A separate security experiment with a defined attacker and access assumptions |

Record success, failures, tool sequence, unnecessary actions, verification quality, latency, and resource usage. Define metrics before scoring. Cost, speed, and capability may trade off; report that rather than collapsing everything into a flattering number.

A reproducibility record should identify the repository commit, generator and harness versions, model identifier and provider, task fixture, public demonstration seed, budget, environment, and evaluation method. Keep private user state out of public records.

No sample size, success threshold, cost budget, or target improvement is approved yet. Establish these when the first task and execution budget are selected.

The first demo should show a complete task, a meaningful comparison, and one limitation. A chart, simulation, or seeded demonstration must be labeled accurately.
