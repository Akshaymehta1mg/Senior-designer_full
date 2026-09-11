# Standalone design skills

This folder contains eight independently invocable Codex skills for pre-UI product-design work. You can call any specialist directly from a raw brief, screenshot, document, question, or existing artifact. No fixed order and no upstream handoff are required.

Each skill stays within its own responsibility. It uses supplied context, labels assumptions, asks only when a missing answer would materially change the result, and may suggest another skill when that would genuinely help. It never calls another skill automatically.

## Skills

| Invocation | Responsibility |
| --- | --- |
| `$design-guide` | Clarify scope and suggest the most relevant specialist when the route is unclear |
| `$context-reader` | Inspect evidence, provenance, analytics integrity, and context without solving |
| `$research-guide` | Decide what must be learned and analyse analytics, conflicting evidence, or competitors |
| `$problem-framer` | Frame the UX problem, supported motivation, user situation, and understanding gaps |
| `$solution-guide` | Compare solution directions and recommend one with trade-offs |
| `$experience-architect` | Define journeys, hierarchy, flow, content, explicit states, and recovery |
| `$wireframe-creator` | Create an interactive Dopamine component-based wireframe |
| `$design-validator` | Independently review a direction, structure, or wireframe |

## Direct use

Invoke the exact skill you need. Examples:

    $problem-framer Frame this UX problem directly from the attached brief and screenshot.
    $solution-guide Compare practical solution directions for this problem.
    $experience-architect Turn this concept into a journey, flow, content hierarchy, and recovery states.
    $wireframe-creator Create an interactive wireframe directly from this brief and the supplied references.
    $design-validator Review this wireframe and identify only material UX failures.

The Design Guide is optional. Use it only when you want help choosing the right specialist.

## Choosing between close specialists

When routing is useful, classify the request by both its decision maturity and the outcome the user needs. This prevents a supplied artifact from being mistaken for the requested deliverable.

| These can look similar | Use the first when | Use the second when |
| --- | --- | --- |
| `$design-guide` / any specialist | The route itself is unclear | The requested specialist or deliverable is already clear |
| `$context-reader` / `$research-guide` | Evidence must be interpreted without deciding what to study | Evidence sufficiency, analytics, conflicting sources, or a research approach must be decided |
| `$research-guide` / `$problem-framer` | The question is whether or how to learn | The supported UX problem and user situation must be articulated |
| `$problem-framer` / `$solution-guide` | The problem must remain open to several solutions | Materially different directions must be compared and one recommended |
| `$solution-guide` / `$experience-architect` | Product role, control model, or direction is undecided | A working direction needs journey, hierarchy, flow, and states |
| `$experience-architect` / `$wireframe-creator` | Experience behaviour needs definition without a visual artifact | An interactive Dopamine wireframe is explicitly requested |
| `$wireframe-creator` / `$design-validator` | The artifact must be created or revised | The supplied artifact needs an independent verdict without silent editing |

Stages are orientation, not gates. A specialist may be invoked directly, and work may be skipped intentionally when the supplied evidence and requested outcome do not require it.

## How standalone behavior works

- Raw input is accepted; earlier skill outputs are optional context.
- A skill will not block merely because another skill was not called first.
- Safe, reversible gaps are handled with clearly labelled assumptions.
- Material ambiguity produces one focused question or a compact set of related questions.
- Another skill may be recommended when useful, but that recommendation is not a prerequisite.
- An explicit request to create or revise a wireframe counts as wireframe permission.

## Flexible responses

Skills do not use mandatory `Input`, `Thought`, `Output`, or `Next agent to call` headings. Each skill chooses the clearest format for the work and ends with one unmistakable action: answer a question, approve a decision, provide something missing, optionally call a relevant skill, or take no action.

## Folder structure

    standalone model/
    ├── .agents/skills/        # workspace discovery links
    ├── references/            # shared and task-specific guidance
    ├── design-guide/
    ├── context-reader/
    ├── research-guide/
    ├── problem-framer/
    ├── solution-guide/
    ├── experience-architect/
    ├── wireframe-creator/
    └── design-validator/

Open this folder as a Codex workspace so the skills under `.agents/skills` are discovered. Each skill contains `SKILL.md` and UI metadata in `agents/openai.yaml`.

## Scope

The package supports pre-UI product-design work through interactive Dopamine component-based wireframes. It does not claim final UI sign-off, create production design-system implementation or design-to-code output, write PRDs or engineering specifications, estimate delivery, or perform post-development visual QC.

## Sources and attribution

Selected routing, evidence-analysis, research, prototyping, state-modeling, and interaction-pattern guidance was adapted from the MIT-licensed [Owl-Listener Designer Skills Collection](https://github.com/Owl-Listener/designer-skills). See `THIRD_PARTY_NOTICES.md`.
