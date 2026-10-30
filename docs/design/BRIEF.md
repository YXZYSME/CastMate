<!--​‌​‌‌​​‌​‌​‌‌​​​​‌​‌‌​‌​​‌​‌‌​​‌​‌​‌​​‌‌ YXZYS | saeng-il ai [systems] — © YXZYS @ saengil.ai -->
<!-- SPDX-License-Identifier: Apache-2.0 -->
<!-- yxzys:sg:ai -->

# Initial direction

Status: selected project direction; product specification still being finalized.

## Intent

CastMate explores role-conditioned generation and curation of individual agent harnesses. The generated artifact is the operating arrangement around a model: planning loops, tool-selection policies, verification behavior, and selection of lessons.

The owner's example is an agent named Fred with the occupation Systems Engineer. A seed influences its initial behavior and harness construction. Subsequent task outcomes may influence later curation and improvement.

The owner selected the project name CastMate and this direction on 29 October 2026 (America/Chicago), and selected Apache-2.0 for the repository. The intended event track is Indie Developer.

## Selected constraints

- Generate differences in the harness that can affect actual decisions and tool use.
- Preserve the idea of progressive improvement through experience.
- Require an approval hook before downloading or executing a new skill.
- Keep claims about uniqueness and resistance to copying separate from demonstrated facts.
- Preserve public framework code while keeping private instance state out of the repository.

## Proposed first experiment

Use one underlying Meta model, a fixed permitted tool catalog, equal budgets, and synthetic engineering tasks. Generate multiple candidate harnesses. Evaluate capability and stable behavioral differences, then compare with a role prompt and a fixed harness.

A proposed generation pipeline is:

`role + seed → behavior specification → candidate control flow/tool policies → evaluation → curation → versioned execution`

The policy and approval boundary remains outside generated control flow. Harness proposals cannot modify their own permissions or fabricate evaluation success.

These are design proposals, not an implementation claim or approval of a particular architecture.

## Open choices

| Choice | Why it matters |
| --- | --- |
| First user and task | Defines impact and the smallest useful demo |
| Curation objective | Determines whether to favor specialization, quality, diversity, or a constrained combination |
| What the seed controls | Defines reproducibility and meaningful variation |
| Adaptation scope | Determines whether experience changes parameters, graph structure, selected skills, or several of these |
| Exact models and deployment | Determines runtime policy, cost, license obligations, and repeatability |
| Implementation language and interface | Determines the application structure and delivery path |
| Meaning of “one of one” | Distinguishes unique issuance, different behavior, protected identity, and copying resistance |
| Protection mechanism and recovery | Determines key custody, execution boundary, and how instances survive device loss |

No technology stack, model checkpoint, hardware guarantee, model-training method, or uniqueness guarantee is selected here. The project does not currently analyze real people's personalities.
