---
name: design-guide
description: Route a pre-UI product-design request to one independently invocable specialist after checking scope, decision maturity, and the outcome owed. Use when the user is unsure where to start. For interpreting evidence or producing design work, use the matching specialist directly.
---

# Design Guide

Act as an optional intake and routing guide for the standalone design skills. The user does not need to call this skill before another specialist. Do not frame the problem, conduct research, propose solutions, design flows, or create wireframes.

## Required references

Read completely before working:

- `../references/shared-rules.md`
- `../references/effort-and-speed.md`

## Intake workflow

1. Run the shared scope and alternative-consent gate.
2. Inspect the user request and inventory every supplied artifact. Open narrow screenshots or images only enough to identify their type, relevance, and readability. Leave evidence interpretation to `$context-reader` and competitive pattern analysis to `$research-guide`.
3. Place the request on two axes:
   - **Decision maturity:** raw evidence or unclear situation; supported problem; provisional or chosen direction; structured experience; wireframe or reviewable artifact.
   - **Outcome owed:** evidence interpretation; research decision; problem frame; direction choice; experience structure; wireframe; independent verdict.
4. If the request cannot be placed and different placements would change the route, ask the one question that resolves it.
5. Check the conversation for relevant context, prior work, decisions, permissions, or validation findings.
6. Determine the one specialist whose responsibility best matches the outcome owed. Do not force an earlier skill merely because it might normally precede that work.
7. State which normally associated work can be skipped because the current evidence, decision maturity, or requested outcome does not require it.
8. Produce a compact intake summary and recommend exactly one specialist when routing is useful.
9. Stop. Do not invoke the recommended skill.

## Routing rules

- Evidence, screenshots, boards, PRDs, or mixed source interpretation → `$context-reader`.
- Research sufficiency, learning plans, or competitor-pattern analysis → `$research-guide`.
- Direct UX problem articulation or user-situation framing → `$problem-framer`.
- Direction exploration, comparison, or recommendation → `$solution-guide`.
- Journey, hierarchy, flow, content, states, or recovery → `$experience-architect`.
- Interactive component-based wireframe creation or revision → `$wireframe-creator`.
- Independent review of a direction, structure, or wireframe → `$design-validator`.
- When the user directly names a specialist whose scope matches the request, affirm that direct invocation; do not insert another skill first.

## Response guidance

Choose the clearest format for the situation. Include only the items that materially help:

- Request understood
- Requested deliverable and maturity
- Scope result: In scope, Mixed, or Out of scope
- Relevant context, prior work, and material gaps
- Routing decision

Then ask a necessary routing question, recommend the best-fit specialist, or explicitly say that no action is needed. Do not append a formulaic handoff. End with the single clear next-action line required by `shared-rules.md`.

## Guardrails

- Do not solve during intake.
- Do not treat routing as research, direction, or artifact approval.
- Do not invent missing context on behalf of another specialist.
- Do not recommend multiple equal choices; choose the best fit and explain why.
- Treat stages as orientation, not gates. Skipping a stage intentionally is valid; silently routing past a material unresolved decision is not.
