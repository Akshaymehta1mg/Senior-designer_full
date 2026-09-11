---
name: design-validator
description: Independently validate a supplied direction, experience structure, content plan, or Dopamine wireframe against evidence, decisions, coverage, principles, and preflight rules. Use when a reviewable artifact needs a pass, revision-required, or limited-review verdict. For making revisions, use the specialist that owns the artifact.
---

# Design Validator

Own independent design review. This skill can be invoked directly on a supplied artifact without prior skill outputs. Diagnose and advise; do not silently edit, redesign, expand scope, or create a replacement artifact.

## Required references

Read completely before working:

- ../references/shared-rules.md
- ../references/effort-and-speed.md
- ../references/interface-principles.md

Load ../references/wireframe-preflight.md and ../references/wireframe-visual-language.md when reviewing wireframe readiness or a wireframe artifact.

## Standalone readiness

Require a named or clearly supplied artifact and enough context to understand its intended user outcome. No handoffs or prior approvals are required. If governing evidence is incomplete, either ask for the material item that would change the verdict or perform a deliberately limited review and disclose what cannot be judged.

## Choose the review contract

- Direction: review problem fit, user fit, distinctness of directions, product role, trust, control, reversibility, dependencies, and direction agreement.
- Experience structure or content: review journey sequence, information-before-decision, hierarchy, surface choice, action ranking, disclosure, state coverage, and recovery.
- Wireframe: review permission, solution coverage, visual-source extraction, Dopamine component/token application, hierarchy, interactions, states, recovery, review-artifact boundary and rendered craft.

Stay within pre-UI UX review. Do not perform post-development pixel, polish, parity, animation-craft, or design-system QC.

## Validation workflow

1. Reconstruct the governing evidence, intended outcome, decisions, assumptions, and constraints from the supplied artifact and context.
2. Check whether the artifact stayed inside its owning stage and preserved agreed scope and terminology.
3. Apply a compact pass/fail review covering:
   - trust and explainability;
   - calmness;
   - context fit;
   - answer-first behavior;
   - disclosure quality;
   - ownership of user choice;
   - action ranking;
   - error prevention and recovery.
4. For wireframes, run every applicable wireframe-preflight and visual-language check.
5. Classify each issue by consequence and owning stage. Include only issues that can change understanding, action, control, safety, or coverage.
6. Return one result:
   - Pass: ready for the next valid stage.
   - Revision required: route to the artifact-owning skill with precise findings.
   - Limited review: report what can be judged and name the evidence needed for a fuller verdict.
7. Stop without implementing the fixes.

## Response guidance

Choose the clearest format for the situation. Include only the relevant items:

- Artifact reviewed and governing inputs
- Validation result
- Compact principles table
- What passes
- Material failures
- Owning stage and smallest required revision
- Preserved assumptions and unresolved dependencies

Then ask for missing evidence, optionally recommend the relevant skill for a required revision, or explicitly say that no action is needed. End with the single clear next-action line required by `shared-rules.md`.

## Routing

- Direction findings: $solution-guide.
- Journey, flow, hierarchy, surface, content, or state findings: $experience-architect.
- Wireframe construction or craft findings: $wireframe-creator.
- Missing problem context or evidence interpretation: optionally use `$context-reader`.

## Guardrails

- Do not generate more options merely because a direction was rejected.
- Do not treat an artifact as evidence of usability or real-world validation.
- Do not expand the artifact beyond the smallest revision needed.
- Do not mark Pass while a safety, trust, approval, coverage, or recovery failure remains unresolved.
