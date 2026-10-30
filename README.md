<!--​‌​‌‌​​‌​‌​‌‌​​​​‌​‌‌​‌​​‌​‌‌​​‌​‌​‌​​‌‌ YXZYS | saeng-il ai [systems] — © YXZYS @ saengil.ai -->
<!-- SPDX-License-Identifier: Apache-2.0 -->
<!-- yxzys:sg:ai -->

# CastMate

**Behavior-conditioned generation and curation of agent harnesses.**

CastMate explores whether a role and a random seed can produce a useful individual agent architecture: different planning loops, tool-selection policies, verification strategies, and learning behavior.

**Status: design and repository setup.** No runnable application, trained model, benchmark result, or copy-resistance guarantee is available yet. The initial product plan is being finalized.

The proposed flow is:

`role + seed → behavior specification → candidate harness → evaluation and curation → versioned agent`

Approval hooks remain outside the generated behavior. A generated agent must not be able to grant itself permission to download or execute a new skill.

| Start here | Purpose |
| --- | --- |
| [Initial direction](docs/design/BRIEF.md) | Selected concept, proposed scope, and open decisions |
| [Repository plan](docs/REPOSITORY-PLAN.md) | Organization now and when implementation begins |
| [Decision record](docs/decisions/0001-generated-harnesses.md) | Why the project focuses on generated operating behavior |
| [Research iterations](docs/research/ITERATIONS.md) | Concise ideation history and prior-art references |
| [Evaluation plan](docs/evaluation/PLAN.md) | How the proposed claims will be tested |
| [Hackathon review](docs/hackathon/COMPLIANCE.md) | Requirements, evidence gaps, and current review scope |

This is intended for the **Indie Developer** track of the Meta Global AI Developer Hackathon 2026. Theme selection, exact Meta models, hosting, and implementation language remain open. The repository is not an official Meta project or a certified submission.

A working demo, installation instructions, and measured results will be added when they exist. There are no installation or execution steps at this stage.

Licensed under [Apache-2.0](LICENSE). See [NOTICE](NOTICE) and [third-party notices](THIRD_PARTY_NOTICES.md). The framework's license does not make a generated agent impossible to copy.
