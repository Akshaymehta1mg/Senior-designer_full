---
name: wireframe-creator
description: Create or materially revise an interactive Dopamine component-based wireframe while preserving solution coverage and running design preflight. Use when the user explicitly requests a wireframe from a brief, direction, evidence, or prior UX work. For independent review use `$design-validator`; do not use for final UI sign-off or production implementation.
---

# Wireframe Creator

Own construction and revision of the interactive Dopamine component-based wireframe. Do not claim final UI sign-off, create production implementation, modify the official design-system library, or produce design-to-code output.

## Required references

Read completely before working:

- ../references/shared-rules.md
- ../references/effort-and-speed.md
- ../references/wireframe.md
- ../references/wireframe-visual-language.md
- ../references/wireframe-preflight.md
- ../references/interface-principles.md
- ../references/dopamine-2-wireframe-reference.md

Load ../references/prototype-strategy.md when the prototype question, required fidelity, or scope is not already explicit.

## Standalone readiness

An explicit request to create or revise a wireframe counts as permission. No Solution Guide or Experience Architect output is required. Establish the minimum working direction, user goal, core flow, hierarchy, material states, and constraints from the raw request and supplied evidence. Derive reversible structure with labelled assumptions when safe; ask before inventing a material direction or high-consequence behavior. A request for final UI still requires the scope alternative and user consent described in `shared-rules.md`.

## Mandatory preflight

Before calling a visualization tool, writing HTML, or creating any artifact:

1. Confirm the explicit wireframe request, scope, and evidence boundary.
2. Summarize the working direction, core flow, material assumptions, and unresolved constraints.
3. State the decision the wireframe should support and the riskiest assumption it needs to expose. Keep fidelity no higher than needed to answer that question while meeting the requested interactive-wireframe contract.
4. Build a solution-coverage matrix mapping every required stage, outcome, explanation, action, branch, overlay, and recovery path to a screen, surface, state, or interaction.
5. Apply interface principles and resolve or expose failures.
6. If visual sources were supplied, open every relevant source and produce a concrete source-language extraction covering layout rhythm, density, navigation, proportions and shapes, grouping, hierarchy, action placement, icon treatment, interaction patterns, Dopamine component/token application, and at least three source-specific markers.
7. Run wireframe-preflight.md internally. If any item fails, explain only the blocking design gap and stop.

Do not create manifests, ledgers, JSON orchestration files, or technical preflight artifacts.

## Construction workflow

1. Preserve the agreed solution and terminology. Ask only when construction would materially change it.
2. Start from the familiar category pattern visible in the supplied source. Build one primary screen and no more than four essential alternate, error, or recovery states by default.
3. Give every screen or surface one clear purpose, primary understanding, information hierarchy, action consequence, and next state.
4. Use Dopamine semantic colours, typography, spacing, radii, elevation and documented component states. Derive product-family resemblance from supplied screens without claiming pixel accuracy.
5. Connect only interactions needed to explain the UX logic, including meaningful back, change, cancel, retry, undo, overlay, branch, and recovery behavior.
6. Use functional motion only when it clarifies a state change.
7. Inspect the rendered artifact once and revise material craft failures.
8. Deliver the artifact as an interactive Dopamine component-based wireframe with concise assumptions and unresolved dependencies.

## Optional follow-on

- `$design-validator` can independently review a completed wireframe.
- Apply validator findings by rerunning this skill.
- If a requested revision requires unresolved direction or structural work, optionally recommend `$solution-guide` or `$experience-architect`.

## Response guidance

Choose the clearest format for the situation. Present only what materially helps review the artifact:

- Journey context
- Solution-coverage matrix
- Source-language extraction when sources exist
- Screen and surface map
- States and recovery
- Interaction and motion notes
- Design notes, assumptions, and UI handoff boundary
- Link or path to the wireframe artifact

Then ask a necessary question, optionally recommend validation or a relevant specialist, or explicitly say that no action is needed. End with the single clear next-action line required by `shared-rules.md`.

## Guardrails

- Never claim pixel-perfect, final, production or usability-validation accuracy.
- Do not add a notes board or large custom application unless explicitly requested.
- Do not ignore unreadable or insufficient visual references; request a usable source.
- Do not let supporting rationale compete visually with the wireframe.
- Do not turn business taxonomy into separate sections unless users must understand or act on those distinctions.
- Remove any section, control, state, or overlay that does not prevent or recover from a named user failure.
