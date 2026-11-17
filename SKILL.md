---
description: Design and implement polished, human-crafted interfaces
  that avoid generic AI-generated UI patterns. Use when building,
  redesigning, or refining web or app interfaces.
name: human-like-ui-design
---

# Human-Like UI Design Skill

## Purpose

Create interfaces that feel intentionally designed by a thoughtful
product designer---not like a generic template or an automatically
generated dashboard. Prioritize clarity, personality, usability, visual
hierarchy, and consistency.

This skill applies to web apps, dashboards, landing pages, portfolios,
admin panels, and mobile-responsive interfaces.

## Core principles

1.  **Design for the product, not for trends.** Understand the product's
    audience, purpose, and primary task before choosing a visual
    direction.
2.  **Give the interface a distinct identity.** Choose a coherent visual
    concept, typography system, spacing rhythm, and restrained color
    palette.
3.  **Make usability the priority.** Every visual decision should
    improve comprehension, navigation, feedback, or task completion.
4.  **Use restraint.** Avoid adding decoration, cards, gradients,
    shadows, icons, or animations without a clear purpose.
5.  **Build real interfaces.** Use working navigation, meaningful
    states, realistic content, and functional controls---not static
    mockup-like elements.

## Avoid generic AI-generated UI

Do not default to: - Purple/blue gradients on every page. - A giant
centered heading followed by three identical feature cards. - Excessive
rounded cards, pill buttons, glassmorphism, and floating blobs. -
Repeating the same card layout for unrelated content. - Emoji as a
substitute for a considered icon system. - Arbitrary decorative charts,
statistics, badges, or testimonials. - Overuse of shadows, borders,
gradients, and accent colors. - Huge empty hero sections or unnecessary
whitespace. - Generic copy such as "Unlock your potential" or "The
future starts here." - Fake functionality, placeholder links, or buttons
that do nothing.

These patterns are not forbidden when they genuinely suit the product.
Avoid using them as automatic defaults.

## Start with a design direction

Before implementation, briefly establish:

-   Product type and target audience.
-   The most important user task on the page.
-   A suitable visual personality (for example: editorial, technical,
    playful, premium, utilitarian, calm, or bold).
-   A small color system with accessible contrast.
-   A typography pairing or a single strong type family.
-   Layout structure and responsive behavior.

If the user has supplied a design, screenshot, brand guide, or existing
codebase, treat it as the source of truth. Do not replace established
design decisions without permission.

## Visual design rules

### Layout and hierarchy

-   Establish one clear primary action per view where possible.
-   Use alignment, spacing, scale, and contrast to establish hierarchy.
-   Prefer purposeful asymmetry and varied composition over repetitive
    grids.
-   Group related controls and information; separate unrelated content.
-   Keep line lengths comfortable for reading.
-   Use consistent spacing tokens rather than arbitrary values.
-   Make the first viewport communicate what the product is and what the
    user can do.

### Typography

-   Use a clear type scale with distinct roles for display, headings,
    body, labels, and metadata.
-   Avoid using too many font families or weights.
-   Do not make every heading oversized or every label uppercase.
-   Use readable body sizes and line heights.
-   Use tabular numerals for data-heavy values when appropriate.
-   Load external fonts only when the project permits it; otherwise use
    a considered system stack.

### Color

-   Define semantic tokens such as background, surface, text, muted
    text, border, primary, success, warning, and danger.
-   Use a restrained palette with one deliberate accent color unless the
    brand calls for more.
-   Maintain WCAG-conscious contrast, especially for small text and
    controls.
-   Do not communicate status through color alone.
-   Support the existing light/dark theme when one is already present.

### Components

-   Create components around meaningful reusable patterns, not merely to
    split markup.
-   Keep button styles consistent and distinguish primary, secondary,
    tertiary, and destructive actions.
-   Use cards only when content belongs in a distinct container.
-   Use borders and shadows sparingly; avoid stacking both without
    reason.
-   Keep form labels visible. Include helpful validation and error
    messages.
-   Use a consistent icon library already installed in the project. Do
    not mix unrelated icon styles.

### Content

-   Use realistic, context-specific labels and sample data.
-   Keep interface copy concise, natural, and specific.
-   Avoid lorem ipsum in finished screens.
-   Make empty, loading, error, success, disabled, and selected states
    intentional.
-   Use human-readable dates, numbers, and units appropriate to the
    audience.

### Motion and feedback

-   Use subtle transitions to clarify state changes, hierarchy, and
    interaction.
-   Respect `prefers-reduced-motion`.
-   Avoid animation that delays common tasks or distracts from content.
-   Provide visible hover, focus, active, disabled, loading, and success
    states.
-   Never rely on hover alone for essential functionality.

## Responsive behavior

-   Design mobile layouts deliberately; do not simply shrink desktop
    layouts.
-   Use fluid sizing and sensible max-widths.
-   Prevent horizontal overflow.
-   Make touch targets comfortably large (aim for roughly 44 × 44 CSS
    pixels).
-   Reflow navigation, tables, forms, and multi-column layouts
    appropriately.
-   Test narrow mobile, tablet, and desktop widths.
-   Keep important actions reachable without awkward scrolling.

## Accessibility

-   Use semantic HTML and correct heading order.
-   Associate form controls with labels.
-   Ensure keyboard navigation and clearly visible focus indicators.
-   Provide accessible names for icon-only controls.
-   Add useful alt text to informative images; use empty alt text for
    decorative images.
-   Use ARIA only when native HTML semantics are insufficient.
-   Check color contrast and reduced-motion behavior.

## Implementation workflow

1.  **Inspect before changing.** Read the existing project structure,
    framework, dependencies, routing, design tokens, and components.
2.  **Preserve existing behavior.** Do not remove features, routes, data
    flows, or working interactions while improving appearance.
3.  **Choose a visual direction.** Make design choices that fit the
    product and its audience.
4.  **Build the full experience.** Include realistic content, responsive
    layouts, and all relevant interaction states.
5.  **Reuse the project's stack.** Do not introduce a new UI framework
    or dependency unless necessary and approved.
6.  **Keep code maintainable.** Use clear component boundaries,
    consistent naming, and centralized design tokens.
7.  **Verify the result.** Run the project and inspect the actual
    rendered UI at mobile and desktop sizes.
8.  **Fix visible defects.** Check alignment, overflow, typography,
    contrast, spacing, broken assets, console errors, and nonfunctional
    controls.

## Project-preservation rules

When working in an existing application: - Do not change the overall
layout, colors, navigation, page structure, or component design if the
user explicitly says to preserve the current UI. - Make only the
requested changes. - Do not replace the user's chosen libraries or
rewrite the app unnecessarily. - Do not invent backend endpoints or data
contracts. - If backend behavior is outside the task, use the existing
API contract and keep UI changes isolated. - Ask before making a major
visual or architectural change that was not requested.

## Final quality checklist

Before finishing, confirm:

-   [ ] The interface has a clear visual identity and suits its product.
-   [ ] The hierarchy is obvious without making everything oversized.
-   [ ] Spacing, typography, colors, and component styles are
    consistent.
-   [ ] The design avoids repetitive, template-like sections.
-   [ ] All visible controls have meaningful behavior.
-   [ ] Loading, empty, error, and success states are handled where
    relevant.
-   [ ] Keyboard focus and accessible labels are present.
-   [ ] The layout works on mobile, tablet, and desktop.
-   [ ] There is no unintended overflow or broken content.
-   [ ] Existing functionality and user-requested constraints are
    preserved.

## Expected response when using this skill

When asked to build or improve a UI: - Briefly state the visual
direction only if useful. - Implement the interface rather than merely
describing a design. - Do not ask questions when sensible design
decisions can be made from the existing context. - If a critical
requirement is genuinely unclear, ask one focused question. - At
completion, summarize the implemented changes and disclose anything that
could not be verified.
