---
name: interaction-patterns
description: Apply focused structural checks when the experience is primarily a form, onboarding flow, or search experience.
---

# Interaction Patterns

## Purpose

Use only the section matching the experience being structured. These are decision checks, not templates that override the product context, evidence, platform conventions, or Dopamine components.

## Forms

- Use a clear reading and focus order; a single-column structure is usually safest unless the relationship between fields justifies another layout.
- Give every field a persistent label. Do not rely on placeholder text as the label.
- Group related fields and make field width communicate the expected kind of input where practical.
- Ask only for information needed at that moment; defer optional collection.
- Choose controls that fit the number and kind of choices rather than forcing everything into text inputs or dropdowns.
- Validate at a point that helps without punishing incomplete typing. Place the message near its source, state what happened, and explain how to recover.
- Preserve entered information across errors and back navigation.
- For consequential submission, provide review, confirmation, or reversal proportionate to the risk.

Do not preselect an answer merely because it is common when the choice affects consent, eligibility, money, health, privacy, or another consequential outcome.

## Onboarding

- Define the first meaningful value the user should reach and remove setup that is not required before it.
- Orient users in context instead of teaching every feature upfront.
- Use progressive onboarding, a setup sequence, sample data, or a short tour according to what must be understood or configured.
- Make optional education dismissible and recoverable later.
- Treat empty states as part of onboarding: explain the space, show the first useful action, and give enough preview to understand the result.
- Cover interrupted setup, returning after a gap, skipped steps, and resumption without lost work.

Do not use completion of an onboarding sequence as proof that users reached value.

## Search

- Clarify what can be searched and preserve the query so it can be refined.
- Decide whether users are retrieving a known item, navigating to a destination, or exploring a category; the result structure should reflect that intent.
- Provide suggestions only when they reduce effort without overwhelming the choice.
- Give each result enough context for a decision and expose relevant filtering or sorting without showing every possible control.
- Make applied refinements visible and individually reversible.
- Design zero-result recovery: repeat the query, suggest corrections or broader terms, and offer a useful alternate path.
- Include loading, partial, stale, permission-limited, error, and empty states when the system can produce them.

Do not treat search as a substitute for understandable information architecture.

## Shared checks

- The primary action and consequence are clear.
- Required understanding appears before a consequential choice.
- System feedback stays close to the action that caused it.
- Keyboard, touch, assistive technology, long content, and realistic data do not break the sequence.
- Every material failure has a recovery path that preserves context where possible.
