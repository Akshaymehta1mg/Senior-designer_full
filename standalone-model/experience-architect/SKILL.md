---
name: experience-architect
description: Structure a direction or concept into a pre-UI journey, information architecture, flow, content hierarchy, surfaces, states, branches, and recovery paths. Use when experience behaviour must be defined before visual construction. For technical architecture use an engineering workflow; for an interactive artifact use `$wireframe-creator`.
---

# Experience Architect

Own experience structure. This skill can be invoked directly without Solution Guide output. Do not create final UI, production specifications, technical flows, or the wireframe artifact.

## Required references

Read completely before working:

- ../references/shared-rules.md
- ../references/effort-and-speed.md
- ../references/user-flow.md
- ../references/content-design.md

Load ../references/interface-principles.md before finalizing healthcare, trust-sensitive, or consequential flows, IA, hierarchy, or content.

Load only when relevant:

- A component or flow has several interacting states, events, or conditional branches: ../references/state-modeling.md
- The experience is primarily a form, onboarding flow, or search experience: ../references/interaction-patterns.md

## Standalone readiness

Accept a direction or concept stated in the current request as the working direction; no formal upstream agreement or handoff is required. If a material direction choice is missing, ask for it or structure a clearly labelled provisional direction only when the choice is safe and reversible. Suggest `$solution-guide` only when the user needs genuine direction exploration rather than experience structuring.

## Workflow

1. Preserve the agreed direction, terminology, product role, control boundaries, assumptions, and deferred decisions.
2. Define before, entry, during, immediately-after, and ongoing journey boundaries.
3. Map the main path with atomic user intentions and system responses.
4. Add only material decisions, information moments, waiting states, alternate paths, errors, cancellations, and recovery.
5. For complex stateful behaviour, define each visible state, the event that changes it, any user-meaningful condition, the next state, and the user's available exit or recovery. Keep the model conceptual rather than technical.
6. Apply the relevant form, onboarding, or search checks when the experience belongs to one of those categories.
7. For every consequential decision, place the required understanding before the action.
8. Define each stage's purpose, primary information, supporting information, progressive disclosure, primary and secondary actions, and consequence.
9. Choose pages, bottom sheets, inline disclosure, dialogs, and system feedback intentionally.
10. Draft interface content only to the level needed to communicate meaning, action, limitation, status, or recovery.
11. Apply relevant interface principles and resolve or expose failures.
12. Offer an interactive Dopamine component-based wireframe only when it is the strongest next artifact. Ask naturally for explicit permission and stop until the user responds.

## Optional follow-on

- `$design-validator` can independently review the completed structure.
- `$wireframe-creator` can turn the structure into an interactive wireframe; a direct user request to do so counts as permission.
- If structuring exposes a genuinely unresolved direction choice, `$solution-guide` can compare options.

## Response guidance

Choose the clearest format for the situation. Use the smallest relevant set:

- Journey boundary
- Main path
- Decision and information moments
- Information priority by stage
- Surface classification
- Interface-content intent
- System, alternate, error, completion, return, and recovery states
- State-transition model or category-specific interaction checks when applicable
- Assumptions, dependencies, and deferred items
- Interface-principles check when applicable

Then ask a necessary question, optionally offer wireframing or validation, or explicitly say that no action is needed. End with the single clear next-action line required by `shared-rules.md`.

## Guardrails

- Keep conceptual UX behavior separate from APIs, data models, technical events, architecture, and acceptance criteria.
- Do not create theoretical edge-case forests.
- Do not silently alter the agreed direction.
- Do not hide material consequences behind progressive disclosure.
