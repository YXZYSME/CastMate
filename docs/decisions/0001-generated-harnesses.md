<!--​‌​‌‌​​‌​‌​‌‌​​​​‌​‌‌​‌​​‌​‌‌​​‌​‌​‌​​‌‌ YXZYS | saeng-il ai [systems] — © YXZYS @ saengil.ai -->
<!-- SPDX-License-Identifier: Apache-2.0 -->
<!-- yxzys:sg:ai -->

# 0001 — Focus on generated agent harnesses

Recorded: 29 October 2026 (America/Chicago).
Status: accepted direction; mechanism and implementation remain open.

## Context

The idea began with occupation-driven behavior for a persistent agent. Later discussion explored individual identity and protection against copying. The selected direction places individuality in how an agent's operating harness is generated and curated.

## Decision

Investigate behavior-conditioned, seeded generation of planning loops, tool-selection policies, and other operating choices. Evaluate whether the resulting agents are useful and measurably different.

Keep approval enforcement outside generated behavior. Treat encryption and copying resistance as separate questions that need a defined threat model and evidence.

## Consequences

Research should test actual execution behavior. Different names, seeds, hashes, or prompt descriptions alone do not establish useful individuality.

The open-source framework can be inspected and reused under Apache-2.0. Private instance secrets remain separate. No claim that licensing or encryption makes a harness impossible to reproduce is accepted.

Further decisions belong in later records, with explicit status and evidence. This record does not select the implementation stack or authorize spending.
