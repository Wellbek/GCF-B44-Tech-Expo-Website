# Design System Document

## 1. Overview & Creative North Star: "The Living Archive"

This design system serves as a digital bridge between institutional authority and urgent environmental action. The **Creative North Star is "The Living Archive."** Unlike static institutional portals, this system feels breathable, layered, and high-impact. It rejects the "template" look in favor of an editorial layout that mimics high-end sustainability journals—using intentional asymmetry, pixelated "Ripple" textures, and a rigorous adherence to tonal depth.

We break the rigid grid not by ignoring it, but by mastering it. Images and text should occasionally overlap or bleed across grid lines to create a sense of momentum, while the "Ripples" graphics provide a digital-organic texture that suggests fluid movement and global connectivity.

---

## 2. Colors: Tonal Ecology

The palette is rooted in the "Emerald" (#1B9440) and "Deep Forest" (#0B351A) of the natural world, punctuated by the "Neon Green" (#CBFD3C) of urgent innovation. 

### The Palette
*   **Primary:** `#006B29` (Emerald) - Our core brand anchor.
*   **Secondary:** `#4F6700` (Olive-Neon) - Used for high-impact accents.
*   **Surface:** `#EAFFE9` (Mint Tint) - The base canvas for the digital experience.
*   **On-Surface:** `#00210C` (Deep Forest) - Used for maximum legibility in typography.

### Color Rules for Premium Execution
*   **The "No-Line" Rule:** 1px solid borders are strictly prohibited for sectioning. Structural boundaries must be defined solely through background color shifts. For example, a `surface-container-low` section sits directly against a `surface` background to create a clean, modern break.
*   **Surface Hierarchy & Nesting:** Treat the UI as physical layers of fine paper. Use `surface-container` tiers (Lowest to Highest) to define importance. An inner card should use `surface-container-highest` while its parent section uses `surface-container-low`.
*   **The "Glass & Gradient" Rule:** To provide visual "soul," use semi-transparent surface colors with a `backdrop-blur` (Glassmorphism) for floating navigation or overlays. Main CTAs should utilize a subtle gradient from `primary` (#006B29) to `primary-container` (#008736).

---

## 3. Typography: Institutional Impact

The typographic voice is a dialogue between the industrial geometry of **Space Grotesk** and the human-centric clarity of **Satoshi**.

*   **Display & Headlines (Space Grotesk):** These are our "Voice of Authority." Use `display-lg` (3.5rem) for hero statements. High contrast in scale is encouraged; a massive headline paired with a small, precise label creates an editorial, premium feel.
*   **Body & Titles (Satoshi):** Satoshi provides the "Voice of Reason." It is engineered for long-form readability. Body text should maintain a generous leading (line-height) to ensure an open, inviting feel.
*   **Labels (Space Grotesk):** Used for metadata, chips, and small caps. This maintains the brand's "Tech-Institutional" edge even at small sizes.

---

## 4. Elevation & Depth: Tonal Layering

We do not use structural lines to separate thoughts. We use light and atmosphere.

*   **The Layering Principle:** Depth is achieved by stacking `surface-container` tokens. Avoid drop shadows on standard cards. Instead, a `surface-container-lowest` card on a `surface-container-low` background creates a "soft lift."
*   **Ambient Shadows:** If a floating element (like a modal) requires a shadow, it must be extra-diffused. Use a 24px-48px blur at 4% opacity, tinted with the `on-surface` color (#00210C) rather than pure black.
*   **The "Ghost Border" Fallback:** If a border is required for accessibility, use the `outline-variant` token at 15% opacity. Never use 100% opaque borders; they clutter the "Living Archive" aesthetic.
*   **Ripples & Overlays:** Incorporate the pixelated/blurred "Ripples" graphics as background overlays behind transparent surface layers. This creates a sense of looking through water or atmosphere, adding profound depth to the layout.

---

## 5. Components

### Buttons
*   **Primary:** Solid `primary` (#006B29) with `on-primary` (#FFFFFF) text. Sharp corners (0px radius) to reflect the institutional grid.
*   **Secondary:** `secondary-container` (#C2F432) with `on-secondary-container` (#546D00) text. High visibility for secondary actions.
*   **Tertiary:** Ghost style. No background, `primary` text, with a "Ripples" inspired hover state (subtle background tint).

### Cards & Lists
*   **Forbid Dividers:** Do not use horizontal lines to separate list items. Use vertical white space from the Spacing Scale (e.g., `spacing-6` or `2rem`) or alternating surface tints.
*   **Editorial Cards:** Use large typography and ample padding (`spacing-8`). Images within cards should follow the "Ripples" aesthetic, perhaps featuring a gradient overlay on one edge to blend into the card's surface color.

### Input Fields
*   **Style:** Minimalist. A bottom-only "Ghost Border" using `outline-variant` at 20% opacity. Upon focus, the border becomes the `primary` emerald color. Labels use `label-md` in Space Grotesk for a technical, precise look.

---

## 6. Do's and Don'ts

### Do
*   **Do** use the Spacing Scale rigorously to create "breathing room." High-end design is defined by what you *don't* fill.
*   **Do** overlap the "Ripples" graphics across container boundaries to break the boxy feel of the grid.
*   **Do** use Neon Green (#CBFD3C) sparingly—only for the most critical calls to action or data points.

### Don't
*   **Don't** use rounded corners. This system is built on a 0px radius scale to maintain a sharp, architectural, and institutional feel.
*   **Don't** use grey. All "neutrals" in this system are tinted with green to maintain the "Living Archive" atmosphere.
*   **Don't** center-align long-form body copy. Stick to a sophisticated, left-aligned editorial grid to maintain authority.