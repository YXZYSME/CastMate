<!--​‌​‌‌​​‌​‌​‌‌​​​​‌​‌‌​‌​​‌​‌‌​​‌​‌​‌​​‌‌ YXZYS | saeng-il ai [systems] — © YXZYS @ saengil.ai -->
<!-- SPDX-License-Identifier: Apache-2.0 -->
<!-- yxzys:sg:ai -->

# Model inventory

Status: planned uses only; no model integration or inference has been verified.

The project will conservatively follow the Regulator P08/P09 interpretation while its S9 provenance limitation remains explicit in [SOURCES.md](SOURCES.md). Exact model origin, checkpoint/version, provider, license, data treatment, and each call path must be recorded before implementation is assessed.

| Possible use | Phase | Model / provider | Current status |
| --- | --- | --- | --- |
| Role-to-behavior specification and candidate proposal | Product runtime if generated in the app | Unselected Meta model / unselected provider | Proposed |
| Agent reasoning and tool selection | Product runtime | Unselected Meta model / unselected provider | Proposed |
| Lesson extraction or adaptation | Product runtime if included | Unselected; any model call must be inventoried | Open |
| Candidate assessment | Runtime when part of the product | Prefer task checks where suitable; model judge undecided | Open |
| Embeddings, routing, fallback, reranking, moderation | Depends on actual implementation | No component selected | Review every added call |
| Coding and development review | Development outside product runtime | Developer tooling; operational details kept outside the app | Does not establish Meta product use |

An application feature remains product runtime even if named a test, evaluator, verifier, or background job. A compatible API client does not establish the origin of the model behind it.

Deterministic generation controls, permission checks, cryptography, and ordinary storage are not themselves model calls. Their interfaces still need review for hidden inference dependencies.

Do not put development credentials, Regulator/JEV sidecars, or their configuration into the submitted application's runtime. Do not claim a working model integration from a README, import, package name, or planned table.

When the stack is selected, replace proposed rows with the complete actual inventory, and link sanitized call-path evidence. Model and provider terms must be checked for the exact delivery route; Apache-2.0 does not replace their licenses.
