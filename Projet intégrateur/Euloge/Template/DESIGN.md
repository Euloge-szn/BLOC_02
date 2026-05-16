---
name: NexaLab Innovation System
colors:
  surface: '#18120a'
  surface-dim: '#18120a'
  surface-bright: '#40382d'
  surface-container-lowest: '#130d06'
  surface-container-low: '#211b11'
  surface-container: '#251f15'
  surface-container-high: '#30291f'
  surface-container-highest: '#3b3429'
  on-surface: '#eee0d1'
  on-surface-variant: '#d6c4ac'
  inverse-surface: '#eee0d1'
  inverse-on-surface: '#372f25'
  outline: '#9f8e79'
  outline-variant: '#514533'
  surface-tint: '#ffba44'
  primary: '#ffc56c'
  on-primary: '#442c00'
  primary-container: '#f0a500'
  on-primary-container: '#5f3f00'
  inverse-primary: '#805600'
  secondary: '#44e0c6'
  on-secondary: '#00372f'
  secondary-container: '#07c3ab'
  on-secondary-container: '#004b40'
  tertiary: '#bccfff'
  on-tertiary: '#002e6c'
  tertiary-container: '#93b3fb'
  on-tertiary-container: '#204484'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffddaf'
  primary-fixed-dim: '#ffba44'
  on-primary-fixed: '#281800'
  on-primary-fixed-variant: '#614000'
  secondary-fixed: '#65fae0'
  secondary-fixed-dim: '#40ddc4'
  on-secondary-fixed: '#00201b'
  on-secondary-fixed-variant: '#005046'
  tertiary-fixed: '#d8e2ff'
  tertiary-fixed-dim: '#aec6ff'
  on-tertiary-fixed: '#001a43'
  on-tertiary-fixed-variant: '#214585'
  background: '#18120a'
  on-background: '#eee0d1'
  surface-variant: '#3b3429'
typography:
  display-xl:
    fontFamily: Space Grotesk
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1280px
  gutter: 24px
  margin-desktop: 64px
  margin-mobile: 20px
---

## Brand & Style

This design system is engineered to position the product as a premier gateway for African enterprise digital transformation. The brand personality is authoritative yet forward-leaning, blending the reliability of a high-end financial institution with the agility of a deep-tech incubator.

The visual direction utilizes **Glassmorphism** and **Corporate Modern** styles. It leverages depth through semi-transparent layers and luminous accents to evoke a sense of digital "frontier" technology. The aesthetic is intentionally dark to minimize ocular strain for intensive data work while allowing high-contrast action colors to guide user flow with surgical precision.

## Colors

The palette is anchored in **Abyss (#0D1B2E)**, providing a vast, stable foundation. Surfaces use **Deep Sea (#152B4A)** to create clear container boundaries without breaking the dark-mode immersion. 

**Amber (#F0A500)** is reserved strictly for primary calls to action, progress indicators, and critical highlights. **Teal (#00C2AA)** serves as the "Tech" accent, used for data visualizations, success states, and innovative feature callouts. **Cobalt (#1B4080)** acts as the structural connective tissue, used for borders and inactive states to maintain a high-density, professional appearance.

## Typography

This design system utilizes a dual-font strategy to balance technical edge with human-centric readability. **Space Grotesk** is used for headlines to convey a geometric, futuristic tone appropriate for an innovation lab. Its idiosyncratic glyphs provide a unique brand signature.

**Plus Jakarta Sans** is employed for all body and UI text. Its soft, rounded terminals provide a necessary counterbalance to the sharp geometry of the headings, ensuring that long-form content remains approachable. For data-heavy labels, use `label-sm` with increased letter spacing to ensure maximum legibility at small scales.

## Layout & Spacing

The layout follows a **12-column fluid grid** for desktop, transitioning to a **4-column grid** for mobile. A strict 8px base unit (the "Innovation Grid") governs all spatial relationships. 

Generous negative space is a core requirement of this design system to maintain a premium feel. Content blocks should be separated by at least 64px (8 units) on vertical axes to allow the technical elements room to "breathe." Containers use a maximum width of 1280px to prevent line lengths from becoming illegible on ultra-wide monitors.

## Elevation & Depth

Depth is established through **Tonal Layering** and **Subtle Glassmorphism**. Elements should not use traditional drop shadows. Instead, elevation is communicated by:

1.  **Backdrop Blurs:** High-elevation components (modals, floating menus) should use a 12px blur with a 60% opaque Deep Sea background.
2.  **Inner Glows:** To simulate light hitting an edge, use a 1px top-border with 10% opacity white.
3.  **Luminous Borders:** Active containers use the Cobalt border with a subtle 4px outer glow matching the accent color (Amber or Teal) at very low (15%) opacity to suggest "energy" flowing through the component.

## Shapes

A consistent **8px (0.5rem) border radius** is applied to all standard UI components including cards, buttons, and input fields. This "Rounded" setting strikes a balance between professional rigidity and modern friendliness. 

Interactive elements such as Chips or Tags may use a "Pill" radius (full rounding) to differentiate them from structural layout components. Overlays and Modals should maintain the 8px radius but may increase to 16px (rounded-lg) if they serve as the primary focal point of the viewport.

## Components

-   **Buttons:** Primary buttons use a solid Amber background with black text for maximum contrast. Secondary buttons use a Cobalt outline with Teal text.
-   **Cards:** Cards are the primary container. They feature a 1px Cobalt border, the Deep Sea surface color, and a subtle background blur when positioned over images or complex gradients.
-   **Inputs:** Input fields use a darker shade of Abyss for the background to create a "inset" look, with Cobalt borders that transition to Teal upon focus.
-   **Data Visualization:** Use Teal for positive growth and Amber for points of interest or warnings.
-   **Glass Panels:** Use for sidebars and navigation headers to maintain a sense of depth and context as the user scrolls content underneath.
-   **Innovation Badges:** Small, high-contrast labels used to denote "Beta" features or "New" tech modules, utilizing the Teal accent color.