# Dopamine 2.0 wireframe reference

Use this reference for every component-based wireframe created by these skills, including Tata 1mg, 1mg Labs, Quick Commerce, Care Plan, and Corporate work.

This is a wireframe construction guide distilled from `Dopamine 2.0 — 1mg Design System.zip`. It records reusable layout, hierarchy, component, token, content, icon, and asset patterns. It does not replace a supplied product screen, an agreed UX direction, or the production design system.

## Source and confidence

- Source archive: `Dopamine 2.0 — 1mg Design System.zip`
- Foundation source in archive: `uploads/Dopamine 2.0 design system - base tokens.md`
- Supporting sources: `README.md`, `colors_and_type.css`, component previews, the 1mg JSX UI kit, official logo SVGs, product images, and the design-system manifest
- Foundation tokens are described by the archive as 1:1 with the exported foundation specification.
- The archive states that its UI-kit component visuals are modeled on known 1mg screens and foundation tokens, but are not guaranteed to be pixel-perfect without the original Figma component library or product codebase.
- Hugeicons is the required substitute when the official product icon set is unavailable.
- Category illustrations are not included; placeholders should not be mistaken for official illustrations.

## Source priority for a wireframe

Use evidence in this order:

1. Product screenshots, flows, or boards supplied for the task.
2. Repeated visual and interaction patterns visible in those sources.
3. The Dopamine 2.0 patterns in this reference.
4. Familiar mobile-platform conventions.

Do not force a design-system pattern when it conflicts with the supplied journey, reduces clarity, or hides a material consequence. Preserve product-family resemblance without claiming pixel accuracy.

## Wireframe fidelity boundary

The wireframe should use Dopamine 2.0 rules and component treatments rather than a grayscale translation.

- Use the documented semantic colours, Figtree typography, spacing scale, radii, borders, elevation and component states.
- Reuse Dopamine component patterns for buttons, fields, alerts, chips, cards, navigation, sheets and sticky actions.
- Preserve proportions, grouping, hierarchy, action placement and interaction behavior from supplied product sources.
- Use real product copy and realistic values when they help reviewers understand the flow.
- Keep the artifact reviewable and assumption-led: it is not a claim of pixel accuracy, production readiness, technical feasibility or final visual sign-off.
- Do not invent missing official components, illustrations, icons or tokens. Label a documented substitution when necessary.

### Semantic component application

| Dopamine role | Wireframe treatment |
| --- | --- |
| 1mg Coral primary action | Coral fill with inverse label using the documented primary-button pattern |
| Wellness Green saving or success | Wellness Green text/surface plus check or offer label |
| Precision Blue information | Precision Blue text/surface plus information icon |
| Vital Red error | Vital Red border/text on the documented error surface with inline recovery |
| Sunshine Yellow warning | Warning surface plus icon, consequence and next action |
| Selected chip or tab | Dopamine selected-chip treatment with explicit selected state |
| Disabled control | Documented disabled surface and content tokens with no action affordance |
| Card boundary | Dopamine border or elevation level appropriate to the surface |

Never rely on colour alone to communicate state. Pair it with a label, icon, shape or action change.

## Product character

Dopamine 2.0 is:

- mobile-first;
- practical and shopping-native;
- friendly without being playful;
- trust-forward and explanation-led;
- dense enough for medicine and diagnostic commerce, but clearly grouped;
- rounded and approachable rather than sharp or ornamental;
- restrained in motion and visual effects.

The product should feel like a helpful pharmacist, not a bubbly marketplace mascot.

## Mobile layout

### Reference viewport and grid

| Property | Value |
| --- | --- |
| Reference viewport | 360px wide |
| Columns | 6 |
| Side margins | 16px |
| Gutter | 8px |
| Approximate column width at 360px | 48px |

Use whole-column spans. Avoid fractional column spans.

For tablet or desktop, retain the 8px gutter baseline and expand side padding to approximately 24–40px rather than changing the core rhythm.

### Common fixed areas

| Area | Reference size or behavior |
| --- | --- |
| Top navigation | Approximately 56px |
| Bottom navigation | Approximately 60px plus safe area |
| Sticky bottom action | Approximately 68px plus safe area |
| Screen side padding | 16px |

Do not stack more than two bottom-anchored layers. Always respect safe-area insets.

### Spacing scale

Use only this spatial scale unless a supplied product source clearly establishes another value:

`0, 2, 4, 8, 12, 16, 20, 24, 28, 32, 36, 40px`

Recommended use:

- 2–4px: tightly related labels, helper text, inline metadata;
- 8px: standard component gap and grid gutter;
- 12px: compact card/input padding;
- 16px: screen edge padding and standard card padding;
- 24–32px: major section separation;
- 36–40px: rare large structural separation.

If a spacing value does not fit this scale, round it to the nearest token.

## Typography

### Families

- Use Figtree for interface headings, titles, labels, forms, buttons, descriptions, and tags.
- Reserve Cabinet Grotesk for oversized display moments at 24px, 36px, or 45px.
- Use the bundled Figtree files when the artifact format supports them. Use a system sans-serif fallback only when Figtree cannot be loaded.
- Do not use Cabinet Grotesk below 24px.

### Weight roles

| Weight | Typical role |
| --- | --- |
| 300 Light | Large display only |
| 400 Regular | Body and supporting descriptions |
| 500 Medium | Workhorse body, controls, and moderate emphasis |
| 700 Bold | Labels, tags, actions, and strong body emphasis |
| 800 Extrabold | Page, section, product, and price emphasis |

### Reference type scale

| Role | Size / line height | Typical weight |
| --- | --- | --- |
| Display large | 45 / 52 | 800 |
| Display medium | 36 / 44 | 300 |
| Display compact | 24 / 32 | 300 or 800 |
| Heading large | 32 / 40 | 400–800 |
| Heading medium | 28 / 36 | 400–800 |
| Heading compact | 24 / 32 | 400–800 |
| Section heading | 18 / 28 | 500–800 |
| Page or prominent title | 22 / 28 | 800 |
| Inline title | 16 / 24 | 800 |
| Compact title | 14 / 20 | 800 |
| Body large | 16 / 24 | 400–700 |
| Body standard | 14 / 20 | 400–700 |
| Body compact | 12 / 16 | 400–700 |
| Tag or micro-label | 11 / 16 | 400–700 |
| Eyebrow | 12 / 16, uppercase, 3px tracking | 700 |

Use sentence case for headings, buttons, and body copy. Reserve uppercase plus letter spacing for short eyebrow or category labels.

## Colour roles for UI handoff

Use semantic roles rather than primitive colour names when annotating a wireframe.

### Core neutral roles

| Semantic role | Token mapping | Value |
| --- | --- | --- |
| Primary content | Cool Neutral 10 | `#181A1F` |
| Secondary content | Cool Neutral 30 | `#414752` |
| Tertiary/placeholder content | Cool Neutral 60 | `#868E9E` |
| Default icon | Cool Neutral 50 | `#626A7A` |
| Primary background | Cool Neutral 100 | `#FFFFFF` |
| Page background | Cool Neutral 97 | `#F7F8FA` |
| Subtle grouped background | Cool Neutral 95 | `#EEF1F5` |
| Subtle divider/border | Cool Neutral 90 | `#DDE2EB` |
| Moderate border | Cool Neutral 80 | `#BEC5D1` |

### Brand and state roles

| Role | Value | Intended use |
| --- | --- | --- |
| 1mg Coral | `#FF5443` | Primary 1mg actions and brand accent |
| Quick Commerce Mauve | `#9D59A8` | Quick-commerce branding |
| Care Plan Red | `#903E38` | Care Plan branding |
| Corporate Horizon Blue | `#086E78` | Corporate/B2B branding |
| Wellness Green | `#308956` | Success, savings, offers |
| Precision Blue | `#0B66AF` | Information and links |
| Vital Red | `#A3111E` | Errors and destructive actions |
| Sunshine Yellow | `#BF9514` | Warning and caution |
| Sunrise Glow | `#ED5213` | Bestseller tags and warm highlights |

Do not use Vital Red for brand emphasis. Do not use pure black for normal body text; use the primary-content neutral.

## Shape and elevation

### Radius

| Radius | Recommended use |
| --- | --- |
| 0 | Full-bleed imagery, tables, tab bars |
| 2px | Micro-tags |
| 4px | Small chips, rating pills, inline labels |
| 8px | Buttons, inputs, small cards, product thumbnails |
| 12px | Standard cards, sheets, panels |
| 16px | Prominent cards, hero blocks, modals |
| 24px | Large cards and bottom sheets |
| 9999px | Pills, avatars, circular controls |

Rounded is the default. A square edge should be an intentional structural choice.

### Elevation

| Level | Reference | Use |
| --- | --- | --- |
| Level 1 | `0 2px 4px rgba(39,43,51,.06)` | Resting clickable cards and tiles |
| Level 1 iY | `0 -2px 4px rgba(39,43,51,.06)` | Light bottom-anchored elevation |
| Level 2 | `0 4px 12px rgba(39,43,51,.08)` | Popovers, hover, floating controls |
| Level 2 iY | `0 -4px 12px rgba(39,43,51,.08)` | Bottom sheets and sticky action surfaces |

Use the documented border or elevation level for the component. Keep elevation purposeful and never stack shadows.

## Component construction patterns

### Page header

- White or primary surface.
- 12px vertical and 16px horizontal padding in the supplied 1mg UI kit.
- Back/navigation icon around 22–24px.
- Page title or current-object title occupies the flexible centre area.
- A subtle bottom divider separates the header from scrollable content.
- Keep secondary actions at the trailing edge and visually weaker than the title.

### Buttons

| Variant | Wireframe representation | Intended use |
| --- | --- | --- |
| Primary | 1mg Coral fill, inverse label | One strongest next action |
| Secondary | Primary background, moderate border, primary-content label | Alternate or reversible action |
| Ghost/textual | No container, underlined or dark label | Details, disclosure, low-emphasis navigation |
| Success | Wellness Green treatment plus check icon and label | Confirmed state |
| Destructive | Vital Red treatment plus explicit destructive label | Remove/cancel with consequence |
| Disabled | Documented disabled background and content tokens, no action affordance | Unavailable action |

Reference proportions:

- Medium button: 14px/20 label, 10px vertical and 16px horizontal padding, 8px radius.
- Small button: 12px label, 6px vertical and 12px horizontal padding, 8px radius.
- Large button: 16px label, 14px vertical and 20px horizontal padding, 12px radius.
- Button labels use strong weight and sentence case.
- Icon-label gap is approximately 6px.
- Pressed state may scale to approximately 0.98; do not use this decorative motion in a static wireframe.

### Inputs and search

- Label: 12px bold/strong, placed above the field.
- Field: 14px body text, 12px internal padding, 8px radius.
- Default border: moderate neutral, 1px.
- Focus: 2px 1mg Coral or the relevant product-brand action outline.
- Error: 2px error outline plus nearby plain-language recovery text.
- Helper gap: 4px from field to helper.
- Search: subtle grouped surface, 8px radius, 10px vertical and 12px horizontal padding, 8px icon-to-input gap.
- Keep validation feedback inline. Do not rely on a temporary toast when the user must recover.

### Standard cards and grouped surfaces

- Standard card: primary/white surface, 12px radius, 16px internal padding.
- Use a subtle border or Level 1 elevation only when the card is interactive or meaningfully above the page plane.
- Use 8–12px gaps between tightly related card elements.
- Use a 24–32px gap between major sections rather than wrapping every section in a card.
- Avoid nested cards.

### Product tile

- Small white tile with 8px radius and 8px internal padding.
- Product image sits in a square area with a subtle background and approximately 6–8px radius.
- Product name: approximately 13px/16, strong weight, one or two lines maximum.
- Pack/form metadata: approximately 11px/14, tertiary emphasis.
- Price: approximately 14px strong; MRP and discount are smaller supporting values.
- Show price, MRP, and saving as one related group.
- Add control is full-width within the tile and clearly separated from product information.
- Product photography should be clean and centred on a white or near-white background.

### Alerts and recovery messages

- Inline alert: 12px padding, 8px radius, 10px icon-to-copy gap.
- Title: approximately 13px strong; explanation: approximately 13px/18.
- State icon is approximately 18px.
- Place the message where the user can act on it.
- Copy sequence: what happened → what it means → what the user can do next.
- Use success, error, warning, and information as semantic roles, not decorative colours.

### Tags, badges, chips, and status

- Tag: approximately 11px/16 bold, 2px vertical and 8px horizontal padding, 4px radius.
- Use tags for short states such as `Bestseller`, `38% off`, `Rx required`, or `Care Plan`.
- Filter chip: approximately 13px medium, 6px vertical and 12px horizontal padding, full-pill radius.
- Selected chips become the highest-contrast state.
- Do not use tags to carry long explanations or consequential eligibility rules.
- Pair status colour with text and, when useful, an icon or dot.

### Bottom sheets and dialogs

- Use a bottom sheet for a bounded task that must retain cart, product, or checkout context.
- Use approximately 24px top radius for a prominent bottom sheet.
- Use the documented scrim around 48% dark opacity.
- Use upward Level 2 elevation only to communicate the sheet’s layer.
- Sheet motion is a functional slide-up of approximately 300ms in final UI.
- A dialog should interrupt only for a bounded, immediate decision; do not use it for browsing or deep comparison.

### Sticky action area

- White/primary surface with a subtle top divider.
- Approximately 12px vertical and 16px horizontal padding plus the bottom safe area.
- Use an upward elevation only when the action surface must remain distinct from content.
- One primary action should dominate. Secondary actions may sit beside it only when both are needed at commitment.
- Avoid stacking sticky action areas with multiple bottom bars.

## Offer, coupon, and savings patterns

The archive’s source inventory includes Coupon, Coupon Widget, Best Price Container, Savings Widget, Discount, Offer, and Amount Widget component families. For wireframes, apply the following Dopamine-consistent hierarchy:

1. Lead with the actual saving or best price for the current cart.
2. Explain what produced that saving.
3. State any condition that can change the outcome before presenting an action.
4. Separate cart discounts, payment-dependent offers, membership savings, and bundle savings when they require different user actions.
5. Present unavailable states as explanations or unlock paths, not as active Apply buttons.
6. Use positive, concrete copy such as `You save ₹250`.
7. Keep terms available through progressive disclosure, but never hide eligibility, payment dependency, expiry, cashback timing, or non-stackability.
8. After a cart or payment change, confirm the recalculated saving in context and preserve an undo/change path when possible.

### Savings block hierarchy

Use this order:

1. Actual saving now.
2. Reason or applied offer.
3. Additional conditional saving.
4. Primary action or current applied state.
5. Conditions and terms.

### Representative states

- Best eligible offer applied.
- Eligible alternative with a lower or different outcome.
- Minimum amount or item condition unmet.
- Payment-method-dependent offer.
- Bundle or brand offer.
- Non-stackable offer that would replace another saving.
- Invalid code with inline recovery.
- Offer invalidated after cart or payment change.
- No eligible offer.

## Content and voice

### Tone

- Practical, trust-building, and urgency-aware.
- Short and utility-first.
- Friendly without being playful.
- Use second person: `you`, `your cart`, `your order`.
- Use `we` only when speaking for the brand and that voice is useful.

### Casing and terminology

- Sentence case for headings, buttons, and body.
- Uppercase plus letter spacing only for short eyebrow labels.
- Keep `1mg`, `Tata 1mg`, and `Care Plan` correctly capitalised.
- Use one stable term for each concept across the flow.

### Numbers and money

- Prefix money with `₹` and do not add a space: `₹249`.
- Place strike-through MRP after the current price.
- Frame savings positively: `You save ₹150`.
- Use concrete timing: `Delivery by Tomorrow, 7 PM`, not `Delivery soon`.

### Healthcare restraint

- Do not use emoji in medical or checkout content.
- Do not use false urgency, hype, or marketplace-style pressure.
- Keep clinical caveats in plain language: `Requires prescription`.
- Explain limitations and recovery instead of relying on reassurance alone.

## Iconography and logos

### UI icons

- Use line icons for navigation, inputs, buttons, list actions, and menu items.
- Reference viewbox: 24×24.
- Reference stroke: 2px, rounded caps and joins.
- Icon size: 16–20px inside buttons; approximately 24px in navigation.
- Default icon role maps to Cool Neutral 50; active icons use the relevant action or brand role in final UI.
- Hugeicons is the required substitute, not the official 1mg icon library.
- In a wireframe, use one consistent rounded stroke family; do not mix filled, outlined, emoji, and Unicode icon styles.

### Logos

- The Tata 1mg wordmark assets in the archive are official.
- Primary wordmark artboard: approximately 57×12.
- Labs lockup artboard: approximately 82×12.
- Scale proportionally and keep clear space around the mark.
- Use ink/dark artwork on light surfaces and white artwork on dark or image surfaces.
- The archive explicitly notes that there is no coral wordmark; do not recolour the wordmark coral.
- Use the official bundled logo when brand recognition is part of the screen; otherwise a correctly proportioned labelled placeholder is acceptable.

### Imagery

- Product photography is clean, centred, and studio-lit on white.
- Marketing imagery is warm, human-centred, and practical.
- Category illustrations are flat and colourful in final UI, but the official set is not included in the archive.
- Do not invent category illustrations in a wireframe; use labelled neutral placeholders.

## Motion guidance

Motion should clarify behavior, not decorate the experience.

- Most state changes: approximately 150–250ms with standard easing.
- Bottom sheet or modal: approximately 300ms slide-up/down.
- Reveal: simple opacity change.
- List loading: skeleton treatment rather than a spinner.
- Avoid bounce, spring, parallax, looping, and ornamental motion.
- Respect reduced-motion preferences.

For wireframes, use motion only to explain a sheet, overlay, processing state, confirmation, or undo.

## Wireframe construction recipe

1. Inspect every task-specific screenshot or flow before drawing.
2. Record at least three source-specific visual markers.
3. Map the agreed stages, decisions, branches, explanations, and recovery paths.
4. Start with a 360px mobile frame, 16px side padding, and an 8px rhythm unless the supplied source says otherwise.
5. Give each screen or surface one purpose and one strongest action.
6. Use the type hierarchy to support the user’s decision order.
7. Use 12px standard card radius, 8px control radius, and 24px bottom-sheet radius as defaults.
8. Apply Dopamine semantic colour roles and documented component states.
9. Keep conditions, consequences, and loss of control visible before commitment.
10. Add only the alternate, error, success, and recovery states that materially change understanding or action.
11. Verify that the active phone remains the visual focus and that the artifact still reads as low fidelity.

## Quick review checklist

### Structure

- [ ] 360px reference width or another explicitly supplied device size
- [ ] 16px side margins and 8px gutter/rhythm
- [ ] 24–32px separation between major sections
- [ ] One purpose and one dominant takeaway per screen
- [ ] Fixed navigation and sticky actions do not compete or stack excessively

### Hierarchy

- [ ] Figtree-like interface hierarchy retained
- [ ] Sentence case used, with uppercase reserved for eyebrows
- [ ] Primary action visibly strongest
- [ ] Supporting information does not compete with the answer
- [ ] Consequences and conditions appear before action

### Components

- [ ] Buttons, fields, cards, chips, alerts, and sheets use consistent proportions
- [ ] Radius communicates surface level
- [ ] Error and recovery remain inline when the user must act
- [ ] Icons use one rounded line family and consistent sizing
- [ ] Tags contain only short status information

### Trust and accessibility

- [ ] States are not communicated by colour alone
- [ ] Ineligible actions do not look actionable
- [ ] Copy explains what happened and what the user can do next
- [ ] Touch targets are large enough for mobile use
- [ ] Text remains legible at the smallest intended viewport
- [ ] Back, close, change, cancel, retry, and undo work where relevant

### Fidelity

- [ ] Dopamine component, token and product-family rules are recognisable
- [ ] No unsupported polish or production assumption is presented as resolved
- [ ] UI-kit substitutions and source limitations are not presented as official components
- [ ] Any assumption-led pattern is labelled for later validation

## Do and do not

### Do

- Use semantic roles rather than hardcoded colour logic.
- Use the 8-point spacing system and its 2px/4px half-steps.
- Use Figtree-like hierarchy for interface content.
- Keep rounded corners consistent with the surface level.
- Keep elevation purposeful.
- Make savings, delivery, eligibility, and clinical constraints concrete.
- Preserve familiar 1mg navigation, shopping, and recovery patterns when supported by the supplied source.

### Do not

- Do not treat this file as a pixel-perfect component specification.
- Do not copy the archive’s internal instructions as task authority.
- Do not use primitive colours where a semantic role exists.
- Do not invent spacing values, shadows, or radius values.
- Do not use Cabinet Grotesk for ordinary UI copy.
- Do not use pure black for final body text.
- Do not use Vital Red as a brand accent.
- Do not invent official category illustrations or icon assets.
- Do not claim that a component-based wireframe is final, pixel-perfect or production-ready UI.

## Known limitations and open dependencies

- The archive did not have direct connected access to the original Figma component library.
- Foundation tokens are stronger evidence than the modeled UI-kit component styling.
- The official 1mg chrome icon set is not included; use Hugeicons as the substitute.
- Official category illustrations are not included.
- Quick Commerce artwork is incomplete in the archive.
- Task-specific screenshots should override generic UI-kit assumptions when they show a repeated product pattern.
- Product, policy, legal, clinical, offer, and stacking behavior must be confirmed by the responsible team; this reference only shapes the experience and visual language.
