---
name: Precision Tech & Innovation
colors:
  surface: '#09141e'
  surface-dim: '#09141e'
  surface-bright: '#303a45'
  surface-container-lowest: '#050f19'
  surface-container-low: '#121d27'
  surface-container: '#16212b'
  surface-container-high: '#212b36'
  surface-container-highest: '#2b3641'
  on-surface: '#d9e3f2'
  on-surface-variant: '#c3c5d8'
  inverse-surface: '#d9e3f2'
  inverse-on-surface: '#27313c'
  outline: '#8d90a1'
  outline-variant: '#434655'
  surface-tint: '#b6c4ff'
  primary: '#b6c4ff'
  on-primary: '#002780'
  primary-container: '#3a6afd'
  on-primary-container: '#ffffff'
  inverse-primary: '#104fe4'
  secondary: '#c3c6d6'
  on-secondary: '#2c303c'
  secondary-container: '#454956'
  on-secondary-container: '#b5b8c7'
  tertiary: '#ffb694'
  on-tertiary: '#571f00'
  tertiary-container: '#c95100'
  on-tertiary-container: '#ffffff'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dce1ff'
  primary-fixed-dim: '#b6c4ff'
  on-primary-fixed: '#001550'
  on-primary-fixed-variant: '#003ab3'
  secondary-fixed: '#dfe2f2'
  secondary-fixed-dim: '#c3c6d6'
  on-secondary-fixed: '#171b27'
  on-secondary-fixed-variant: '#434653'
  tertiary-fixed: '#ffdbcc'
  tertiary-fixed-dim: '#ffb694'
  on-tertiary-fixed: '#351000'
  on-tertiary-fixed-variant: '#7b2f00'
  background: '#09141e'
  on-background: '#d9e3f2'
  surface-variant: '#2b3641'
  surface-main: '#00060F'
  surface-elevated: '#242834'
  text-primary: '#FFFFFF'
  text-muted: '#A0AEC0'
  accent-blue: '#3A6AFD'
typography:
  display-lg:
    fontFamily: Montserrat
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Montserrat
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.3'
  headline-lg-mobile:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  body-sm:
    fontFamily: Hanken Grotesk
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 8px
  container-max: 1280px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 48px
---

## Brand & Style

This design system embodies a clean, high-tech aesthetic tailored for industrial and medical software solutions. The brand personality is professional, precise, and forward-looking, emphasizing reliability through a disciplined visual structure.

The design style is **Corporate / Modern** with a lean toward **Minimalism**. It utilizes expansive dark surfaces to create a "command center" feel, balanced by high-contrast typography and strategic accents of electric blue. The interface should feel like a high-performance tool: efficient, unobtrusive, and technologically advanced.

## Colors

The palette is anchored in a "True Dark" philosophy. The primary background (`#00060F`) provides a deep, ink-like canvas that minimizes eye strain and allows data visualizations to pop. 

- **Primary Blue:** Used exclusively for interactive elements, progress indicators, and primary actions. It represents the "energy" of the system.
- **Secondary Slate:** Employed for card backgrounds and container strokes to create subtle depth without breaking the dark aesthetic.
- **Neutrals:** White is reserved for high-priority information and headings, while muted greys handle secondary metadata.

## Typography

The typographic hierarchy prioritizes clarity and technical precision. 
- **Headlines:** Use **Montserrat** for its geometric stability and modern presence. 
- **Body:** **Hanken Grotesk** (selected for its high legibility and contemporary feel) handles all prose and interface text.
- **Technical Labels:** **JetBrains Mono** is introduced for data points, status labels, and IDs to reinforce the industrial/software nature of the product.

Keep line lengths for body text between 60-80 characters to maintain readability against the dark background.

## Layout & Spacing

The system follows a **Fixed Grid** model for desktop to ensure data-heavy interfaces remain organized and predictable.
- **Grid:** 12-column system with a 24px gutter.
- **Rhythm:** An 8px base unit scales all margins and paddings.
- **Adaptation:** On mobile, margins shrink to 16px and the layout reflows to a single column. Information density should remain high but avoid clutter; use generous vertical whitespace between distinct logical sections to allow the user's eyes to rest.

## Elevation & Depth

Depth is communicated through **Tonal Layers** rather than traditional drop shadows. 
- **Base Level:** `#00060F` (The "void" or main background).
- **Raised Level:** `#242834` (Cards, Modals, Popovers).
- **Interaction Layer:** 1px solid borders using an opacity of the Primary Blue (e.g., `rgba(58, 106, 253, 0.2)`) replace shadows to define boundaries.

For critical alerts or modals, a subtle **Glassmorphism** effect may be used (12px background blur with a semi-transparent slate fill) to maintain context of the underlying data while bringing the focus forward.

## Shapes

The shape language is "Soft-Technical." We avoid sharp 90-degree corners to keep the UI approachable, but we also avoid pill shapes to stay professional.
- **Standard Corners:** 4px (0.25rem) radius for buttons and input fields.
- **Container Corners:** 8px (0.5rem) radius for cards and large modules.
- **Icons:** Use linear, 2px stroke icons with slightly rounded terminals to match the font geometry.

## Components

- **Buttons:** Primary buttons use the accent blue with white text. Secondary buttons use a slate border with no fill.
- **Inputs:** Dark fills (`#242834`) with subtle 1px borders. The border should illuminate to Primary Blue on focus.
- **Chips:** Used for status indicators (e.g., "Active", "Processing"). These should be rectangular with the 4px radius and utilize low-opacity background tints of the status color (Success/Green, Warning/Amber).
- **Cards:** No shadows. Define cards using the `#242834` background and a subtle `1px` border to separate them from the base black surface.
- **Data Tables:** Highly condensed, using the `label-caps` typography for headers and a subtle divider line (`rgba(255,255,255,0.05)`) between rows.