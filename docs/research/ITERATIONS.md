<!--​‌​‌‌​​‌​‌​‌‌​​​​‌​‌‌​‌​​‌​‌‌​​‌​‌​‌​​‌‌ YXZYS | saeng-il ai [systems] — © YXZYS @ saengil.ai -->
<!-- SPDX-License-Identifier: Apache-2.0 -->
<!-- yxzys:sg:ai -->

# Research iterations

This is a concise retrospective summary recorded on 29 October 2026 (America/Chicago). The entries describe earlier brainstorming in order; they are not original timestamps or a verbatim transcript.

| Iteration | Idea | Current disposition | Reason / next question |
| --- | --- | --- | --- |
| 1 | Occupation-driven agent behavior, with Fred as a Systems Engineer example | Retained as an input | How does the occupation change actual decisions? |
| 2 | A persistent agent that acquires skills and improves over time | Retained with approval hooks | How are useful lessons distinguished from mistakes? |
| 3 | A “one of one” agent that cannot be replicated | Unresolved research goal | Define what a replica is and what an adversary can access |
| 4 | Seeded generation of the harness itself: loops, tool selection, and behavior | Selected direction | Define the generator and curation objective |
| 5 | Encryption and protected state around the generated harness | Proposed, not selected mechanism | Define threat model, key custody, and recovery before making security claims |

Record new entries only when a hypothesis, scope, or decision changes. Describe failed experiments honestly and link their evidence. Keep the latest direction in [BRIEF.md](../design/BRIEF.md).

## Prior art to examine

- Hu, Lu, and Clune, [Automated Design of Agentic Systems](https://arxiv.org/abs/2408.08435), 2024: explores automated construction of agent systems, including control flow and tool use. This establishes related work, not the novelty or performance of CastMate.
- [NIST SP 800-90A Rev. 1](https://csrc.nist.gov/pubs/sp/800/90/a/r1/final): deterministic random generation is relevant to reproducible seeds. Seed uniqueness is not proof that harness behavior differs.
- [RFC 9334](https://www.rfc-editor.org/rfc/rfc9334.html): background for a possible protected-execution or attestation design. No such design has been selected or implemented.

Public abstract/reference material was consulted during ideation. These references are not dependencies and their implementations have not been imported.

## Publication rule

Publish distilled reasoning, decisions, and rights-cleared findings. Keep raw chats, private discussions, personal data, access tokens, private seeds, and unreleased sensitive material outside Git. Nothing in this log establishes organizer approval or complete originality.
