---
name: wireframe-visual-language
description: Give interactive component-based wireframes a disciplined Dopamine 2.0 visual language derived from the design-system reference and supplied product screens without claiming final or production-ready UI.
---

# Wireframe Visual Language

## Purpose

A component-based wireframe should look deliberate, coherent, and recognisably related to the product without being presented as final or production-ready UI. Use this reference after solution coverage, content hierarchy, and interaction surfaces are agreed.

This is a wireframe construction contract, not a design-system specification or post-development design QC process.

## Source priority

Source inspection is mandatory whenever the user supplies screenshots, product screens, or a flow. Open every relevant frame with the available image or board viewing tool. Do not begin construction until a concrete source-language extraction is visible in the response and confirmed through `wireframe-preflight.md`; generic statements such as “preserve the product style” do not satisfy this gate.

Use visual sources in this order:

1. screenshots, product screens, or flows supplied by the user;
2. patterns repeated across their relevant frames;
3. familiar platform conventions;
4. the Dopamine 2.0 reference and documented component patterns.

Use the documented Dopamine semantic tokens and component patterns. Do not infer missing official components from a single screen or claim pixel-perfect accuracy.

## Apply Dopamine rules and components

When screenshots, product screens, or flows are supplied, inspect every relevant frame and carry forward the repeated visual language:

- information density;
- layout rhythm and screen padding;
- navigation placement;
- component proportions;
- card and container shapes;
- corner-radius character;
- content grouping;
- typography hierarchy;
- placement of primary and secondary actions;
- icon style and sizing;
- bottom-sheet, dialog, and disclosure behavior;
- familiar interaction patterns.

Express those qualities with Dopamine semantic colours, Figtree typography, the 8-point spacing system, documented radii, borders, elevation levels, icons and component states. Treat a flow as evidence of both visual language and cross-screen continuity; do not copy its board layout as interface structure.

Use documented Dopamine treatments for colours, typography, components, official bundled assets, elevation and radii. Do not invent missing official illustrations, icons, components, tokens or production behavior. Lucide remains a documented substitution for the official chrome icon set.

If a supplied pattern would reduce clarity, accessibility, or comprehension in the wireframe, preserve the familiar behavior where possible and note the structural deviation. Do not silently reproduce a weak pattern.

## Semantic token application

| Product treatment | Wireframe treatment |
| --- | --- |
| 1mg primary action | 1mg Coral with inverse label |
| Saving or success | Wellness Green semantic treatment plus explicit label/icon |
| Information | Precision Blue semantic treatment plus explicit label/icon |
| Error or destructive action | Vital Red semantic treatment plus recovery or consequence |
| Warning | Sunshine Yellow semantic treatment plus consequence and next action |
| Selected state | Documented selected chip/tab treatment |
| Disabled state | Disabled background/content tokens with no action affordance |
| Decorative illustration | Use only official supplied assets; otherwise use a labelled placeholder |

Apply colour semantically, not decoratively, and never rely on colour alone.

## Default construction system

Use the product reference to adjust character while keeping these defaults disciplined:

- mobile viewport: `360 × 800px` unless another device is explicitly in scope;
- spacing: an `8px` base rhythm, with `4px` only for tightly related details;
- screen padding: `16px` by default;
- primary action height: `48px`;
- compact controls: at least `40–44px` where interaction is required;
- page title: `20–22px`, semibold;
- section heading: `16–18px`, medium or semibold;
- body: `14–16px`, regular;
- helper or caption: `12px`, regular;
- card and container radius: `12–16px`, adjusted only to reflect the supplied product's general character;
- icons: the official icon set when available, otherwise the documented Lucide rounded-stroke substitute, normally `20–24px`;
- primary action: 1mg Coral fill with inverse label;
- secondary action: primary background with moderate border and primary-content label.

Precise spacing and alignment are required. Pixel-perfect reproduction of the supplied screen is not.

## Artifact presentation

Keep the wireframe itself as the visual focus:

- place the screen-state switcher outside the device frame;
- show one active phone screen at a time unless side-by-side comparison is the explicit purpose;
- center the device frame on the canvas;
- keep the device fully visible at the intended review size;
- use clear selected and unselected switcher states;
- preserve the product's relevant entry or parent context instead of presenting only isolated screens;
- keep design reasoning in a separate notes view, collapsible panel, or secondary tab.

Do not place a permanent explanation panel beside the phone when it competes with the wireframe. Notes may explain the user moment, hierarchy, assumptions, and open decisions, but the product experience remains primary.

## Interaction and motion

Wire the actions necessary to explain the flow. Use simple motion only when it clarifies a state change, overlay, progress change, system response, or recovery. Keep timing restrained and avoid decorative or brand-expressive animation.

## Wireframe craft check

Before delivery, inspect the rendered artifact itself and revise it when needed:

- Is the phone or active screen the main visual focus?
- Is the complete device visible without accidental cropping?
- Are spacing, alignment, grouping, and proportions consistent?
- Is hierarchy clear while brand and semantic colour remain purposeful?
- Are primary and secondary actions visually distinct?
- Are icons consistent in family, size, and stroke?
- Are selected and unselected states immediately understandable?
- Does supporting explanation compete with the product experience?
- Does the wireframe reflect the supplied sources and Dopamine component language?
- Was the mandatory source-language extraction completed before construction began?
- Does the extraction name the inspected sources and at least three details that could only have come from them?
- Does it remain a review artifact and avoid claims of final, pixel-perfect or production-ready accuracy?

This is a self-check of the artifact being created, not design QC of developed software.
