<!--​‌​‌‌​​‌​‌​‌‌​​​​‌​‌‌​‌​​‌​‌‌​​‌​‌​‌​​‌‌ YXZYS | saeng-il ai [systems] — © YXZYS @ saengil.ai -->
<!-- SPDX-License-Identifier: Apache-2.0 -->
<!-- yxzys:sg:ai -->

# CastMate

**Behavior-conditioned generation and curation of agent harnesses.**

CastMate explores whether a role and a random seed can produce useful individual agent architectures with different planning loops, tool-selection policies, verification strategies, and learning behavior.

**Status: design stage.** No runnable application, trained model, evaluation result, or copy-resistance guarantee is available yet. The initial product plan is being finalized.

The proposed flow is:

`role + seed → behavior specification → candidate harness → evaluation and curation → versioned agent`

Approval hooks remain outside generated behavior. An agent must not be able to grant itself permission to download or execute a new skill.

## Project information

- [Development guidance](AGENTS.md) and [contributing](CONTRIBUTING.md)
- [Model integration status](docs/MODEL-USAGE.md)
- [Event contribution record](docs/PROVENANCE.md)
- [Third-party notices](THIRD_PARTY_NOTICES.md)

The intended track is **Indie Developer**, Meta Global AI Developer Hackathon 2026. Theme selection, exact models, hosting, and implementation language remain open. This is not an official Meta project or a certified submission.

Setup instructions, a working demo, and measured results will be published alongside their implementation. The public repository will contain the application code, required runtime assets, tests, and reproducible examples.

Licensed under [Apache-2.0](LICENSE). See [NOTICE](NOTICE). Licensing does not make a generated agent impossible to copy.
