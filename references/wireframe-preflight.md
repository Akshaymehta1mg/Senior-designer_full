---
name: wireframe-preflight
description: Lightweight mandatory readiness check before Senior Designer creates or materially revises a component-based interactive wireframe.
---

# Wireframe preflight

Use this checklist immediately before creating or materially revising a wireframe. This is an internal design-readiness check, not a technical workflow.

Do not create a manifest, ledger, JSON file, task transcript, or separate user-facing artifact. Do not show the checklist when it passes unless the user asks. If an item fails, explain only the design issue that blocks progress and the smallest next action needed.

## Required checks

Confirm all applicable statements:

- The user, goal, journey moment, product context, constraints, evidence, assumptions, and important unknowns are sufficiently understood for this decision.
- The research decision is explicit: move forward, learn first, or proceed provisionally. Do not wireframe while `learn first` remains unresolved.
- The competitive-research decision is explicit: run it because it can change the solution, or skip it with a clear design reason.
- The solution direction is agreed with the user.
- The expected wireframe fidelity and the information or action that should visually dominate are understood.
- The user explicitly permitted wireframe creation.
- The Dopamine 2.0 wireframe reference is loaded and the relevant component and token rules are identified.
- `component-composition-recipes.md` is loaded and the proposed page, list or card, action, feedback, and overlay composition follows it.
- The relevant live catalogue component pages were inspected when accessible; after one failed access attempt, the local Dopamine reference was used as the fallback.
- Every required interaction maps to a documented component family, variant and state or a clearly named component gap.
- Duplicate component-family names were resolved by platform, product context, and current catalogue support rather than by name alone.
- Existing components retain their documented anatomy and are not replaced by generic visual approximations.
- Agreed requirements, stages, screens, states, branches, overlays, recovery paths, and deferred items are mapped in the solution-coverage matrix.
- The compulsory Interface Principles gate passed: the principles served, principle tensions, governing law, and any clarity-or-safety violation were checked.
- Every Interface Principles failure was resolved before construction; a known unresolved violation blocks the wireframe.
- No unresolved issue makes the proposed interaction unsafe, misleading, or structurally unsound.

## Visual-source check

When screenshots, product screens, or flows were supplied, also confirm:

- Every relevant source was opened and visually inspected.
- The source-language extraction identifies layout rhythm, density, navigation, proportions and shapes, grouping, hierarchy, action placement, icon treatment, interaction patterns, and Dopamine component/token application.
- At least three source-specific visual markers are recorded.
- The wireframe uses documented Dopamine semantic colours, typography, spacing, radius, elevation and component states.
- Every applied colour uses a documented semantic or component token from `dopamine-colour-tokens.md`; no component binds directly to a primitive palette or raw hex value.
- Continuous result sets use list rhythm and Dividers unless each item genuinely needs an independent card boundary.
- The proposed hierarchy does not depend on repeating grey fill, border, shadow, and large radius across every item.
- Each current decision has one dominant action; secondary actions do not compete with it.
- The proposal resembles the source product family without claiming pixel-perfect or production-ready accuracy.

When no visual source was supplied, use the live catalogue and the Dopamine construction system in `wireframe-visual-language.md`, `component-composition-recipes.md`, `dopamine-2-wireframe-reference.md`, and `dopamine-colour-tokens.md`; do not invent unsupported product patterns.

## Outcome

- If every applicable check passes, construct the wireframe.
- If a check fails, stop before construction and resolve that specific gap.
- After a material revision, rerun only the checks affected by the change.
