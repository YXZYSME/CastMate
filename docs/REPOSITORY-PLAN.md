<!--​‌​‌‌​​‌​‌​‌‌​​​​‌​‌‌​‌​​‌​‌‌​​‌​‌​‌​​‌‌ YXZYS | saeng-il ai [systems] — © YXZYS @ saengil.ai -->
<!-- SPDX-License-Identifier: Apache-2.0 -->
<!-- yxzys:sg:ai -->

# Repository organization

Status: organization plan for the initial documentation repository, 29 October 2026 (America/Chicago). This is not an approved application implementation plan.

Keep the root focused on orientation, contribution guidance, and licensing. Keep research, design, and submission evidence under docs/. A reader should understand the current project without reading the ideation archive.

## Present organization

```text
CastMate/
├── README.md
├── LICENSE
├── NOTICE
├── AGENTS.md
├── CONTRIBUTING.md
├── THIRD_PARTY_NOTICES.md
├── .brandcontext
├── .gitignore
├── .github/
│   └── PULL_REQUEST_TEMPLATE.md
└── docs/
    ├── REPOSITORY-PLAN.md
    ├── design/BRIEF.md
    ├── decisions/0001-generated-harnesses.md
    ├── research/ITERATIONS.md
    ├── evaluation/PLAN.md
    └── hackathon/
        ├── COMPLIANCE.md
        ├── SOURCES.md
        ├── PROVENANCE.md
        └── MODEL-USAGE.md
```

These are real documents. The initial commit will be the documentation baseline, not proof of a working agent.

## Proposed implementation organization

Create these directories only when the chosen stack and approved product plan need them. Names describe responsibilities; they do not select a programming language or imply separate services.

```text
src/
  generation/       # Role, seed, behavior specification, candidate construction
  curation/         # Candidate evaluation and selection
  runtime/          # Validated harness execution and bounded loops
  policy/           # Approval hooks and deterministic permission checks
  tools/            # Tool catalog, adapters, skill acquisition
  history/          # Versioned lessons, outcomes, and provenance
  protection/       # Established cryptography integration, if selected
app/                 # One demo interface, when its platform is selected
tests/               # Behavioral, integration, and policy regression tests
evals/
  fixtures/          # Reviewed synthetic tasks and public demonstration seeds
  protocols/         # Fixed comparison methods and metric definitions
  results/           # Sanitized results tied to exact commits and model versions
examples/            # Minimal runnable examples, when available
```

Start as one repository and one executable product. Split services or packages only when a demonstrated requirement justifies it. Do not pre-create empty modules or fake package manifests.

## Brainstorming and decisions

Keep a short public record of significant iterations in research/ITERATIONS.md. Record the rationale, status, uncertainty, and next experiment. Do not publish raw chat transcripts or private competitor discussions.

Keep the current direction in design/BRIEF.md. Move accepted choices into numbered decision records; do not silently turn a tentative idea into a requirement. Use issues for bounded work and pull requests for changes. A running stream of half-formed ideas does not belong in the root README.

Use actual dates when recording and committing. A retrospective summary must say that it is retrospective. Git history supports provenance, but commit dates alone do not establish when an invention occurred.

## Build and submission sequence

1. Confirm the first user, task, theme, stack, exact models, and curation objective.
2. Approve a bounded product design and implementation plan.
3. Build a minimal end-to-end loop with policy checks and a synthetic example.
4. Compare it with the baselines in evaluation/PLAN.md.
5. Add exact setup commands, locked dependencies, and an accessible demonstration.
6. Refresh the source ledger and review the submission against COMPLIANCE.md.

Add CI when there is runnable behavior to verify. Keep credentials in deployment or CI secret storage, not workflow files. A green workflow is evidence about its checks, not general product readiness.

## Private instance state

Use .castmate/ or an owner-selected external data directory for local instance state. It is ignored by Git. Store real private seeds, keys, personal memory, and raw traces there only after defining storage protections. A directory name or ignore rule does not provide encryption.

Public examples must use deliberate demonstration seeds and synthetic data. Keep the generated harness version and generator version distinguishable so a test can be reproduced without exposing a user's private instance.
