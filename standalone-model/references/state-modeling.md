---
name: state-modeling
description: Model user-visible experience states and transitions so branches, recovery, and exits are complete without becoming technical architecture.
---

# State Modeling

## Purpose

Use this reference when a component or flow has interacting conditions that a linear happy path cannot express safely. Model only behaviour the user experiences or that changes what the interface must communicate.

## Model elements

- **State:** a distinct user-visible condition such as idle, editing, validating, waiting, success, partial success, empty, unavailable, or error.
- **Event:** a user action, system response, interruption, or passage of time that can change the state.
- **Transition:** the permitted movement from one state to another.
- **Guard:** a user-meaningful condition that changes whether a transition is available, such as missing information, permission, eligibility, or connectivity.
- **Visible response:** what the interface shows, enables, preserves, or explains in the resulting state.

Do not add APIs, services, data models, logging actions, or implementation events.

## Modeling method

1. Start with the main path and its visible states.
2. Add waiting, empty, partial, permission, interruption, cancellation, and error states only when they materially affect understanding or action.
3. For each transition, state the initiating event, any guard, resulting visible state, preserved user work, and available next action.
4. Check that every state has a valid exit, retry, back path, cancellation, or intentionally terminal outcome.
5. Identify impossible combinations and ensure the interface never implies them simultaneously.
6. Map every retained state to a screen, surface, component state, or feedback treatment.

## Compact output

| Current state | Event | Guard or condition | Next state | Visible response | Exit or recovery |
| --- | --- | --- | --- | --- | --- |

Use a diagram only when it communicates branching more clearly than the table.

## Guardrails

- Keep one model focused on one user concern.
- Do not create exhaustive theoretical edge cases.
- Preserve entered information across recoverable failures whenever possible.
- Do not leave waiting, error, or permission states without a user-understandable next step.
