---
name: Kinetic Glass
colors:
  surface: '#031427'
  surface-dim: '#031427'
  surface-bright: '#2a3a4f'
  surface-container-lowest: '#000f21'
  surface-container-low: '#0b1c30'
  surface-container: '#102034'
  surface-container-high: '#1b2b3f'
  surface-container-highest: '#26364a'
  on-surface: '#d3e4fe'
  on-surface-variant: '#bec8d2'
  inverse-surface: '#d3e4fe'
  inverse-on-surface: '#213145'
  outline: '#88929b'
  outline-variant: '#3e4850'
  surface-tint: '#89ceff'
  primary: '#89ceff'
  on-primary: '#00344d'
  primary-container: '#0ea5e9'
  on-primary-container: '#003751'
  inverse-primary: '#006591'
  secondary: '#ddb7ff'
  on-secondary: '#490080'
  secondary-container: '#6f00be'
  on-secondary-container: '#d6a9ff'
  tertiary: '#c0c6db'
  on-tertiary: '#293040'
  tertiary-container: '#949baf'
  on-tertiary-container: '#2c3343'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#c9e6ff'
  primary-fixed-dim: '#89ceff'
  on-primary-fixed: '#001e2f'
  on-primary-fixed-variant: '#004c6e'
  secondary-fixed: '#f0dbff'
  secondary-fixed-dim: '#ddb7ff'
  on-secondary-fixed: '#2c0051'
  on-secondary-fixed-variant: '#6900b3'
  tertiary-fixed: '#dce2f7'
  tertiary-fixed-dim: '#c0c6db'
  on-tertiary-fixed: '#141b2b'
  on-tertiary-fixed-variant: '#404758'
  background: '#031427'
  on-background: '#d3e4fe'
  surface-variant: '#26364a'
typography:
  headline-xl:
    fontFamily: Montserrat
    fontSize: 4rem
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Montserrat
    fontSize: 2.5rem
    fontWeight: '700'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Montserrat
    fontSize: 1.5rem
    fontWeight: '600'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Inter
    fontSize: 1.125rem
    fontWeight: '400'
    lineHeight: '1.7'
  body-md:
    fontFamily: Inter
    fontSize: 1rem
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: Space Grotesk
    fontSize: 0.75rem
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.1em
  mono-code:
    fontFamily: Space Grotesk
    fontSize: 0.875rem
    fontWeight: '400'
    lineHeight: '1.5'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  xs: 0.5rem
  sm: 1rem
  md: 2rem
  lg: 4rem
  xl: 8rem
  gutter: 24px
  max-width: 1280px
---

## Brand & Style

This design system is built for a high-end front-end developer portfolio, blending the precision of technical innovation with the ethereal quality of futurism. The aesthetic centers on **Glassmorphism**, utilizing layered translucency to create depth without clutter. The interface feels like a digital cockpit: advanced, responsive, and meticulously organized.

The emotional response should be one of "sophisticated mastery"—the user should feel they are interacting with a high-performance tool crafted by someone who understands the nuance of modern web capabilities. It avoids heavy, solid blocks in favor of light-refracting surfaces, subtle glows, and razor-sharp typography.

## Colors

The palette is anchored in a deep-space environment. The background is not pure black, but a rich, layered "Deep Tech Blue" that allows for better contrast with glass effects.

- **Primary (Cyan):** Used for critical actions, terminal cursors, and active code states.
- **Secondary (Purple):** Used for high-level creative accents and hover states to provide a sense of "digital mystery."
- **Surfaces:** Utilize varying degrees of opacity (10-40%) over the deep background.
- **Accents:** Vibrant glows are used sparingly to guide the eye toward conversion points (e.g., "Hire Me" or "View Project").

## Typography

This design system uses a triple-font strategy to balance impact, readability, and technical flair.

1.  **Montserrat** is the display powerhouse, providing a geometric, urban authority to large headings.
2.  **Inter** handles the heavy lifting of project descriptions and professional details, ensuring maximum legibility across all devices.
3.  **Space Grotesk** is introduced for labels, metadata, and "tech" callouts to reinforce the futuristic theme through its distinctive geometric shapes.

Text hierarchy is strictly maintained with significant vertical air, allowing the content to breathe.

## Layout & Spacing

The layout follows a **Fixed Grid** philosophy on desktop, centered to provide a curated, gallery-like experience.

- **Grid:** A 12-column system with a generous 24px gutter.
- **Rhythm:** Spacing units are based on a 4px scale. Content sections are separated by `xl` (128px) margins to emphasize the "clean interface" requirement and prevent visual overcrowding.
- **Safe Areas:** Cards and containers utilize internal padding of `md` (32px) to maintain a premium feel.

## Elevation & Depth

Depth is achieved through **optical transparency** rather than traditional shadows.

- **Backdrop Blurs:** Every glass surface must have a `backdrop-filter: blur(12px)`.
- **Layering:** Elements closer to the user have higher opacity backgrounds (e.g., 20% vs 10%) and slightly brighter border-top-colors to simulate a top-down light source.
- **Glows:** Instead of black shadows, use subtle, colored outer glows (10-15% opacity of the Primary color) for active or elevated states.
- **Borders:** "Ghost borders" are essential—1px solid borders with 20% opacity white or primary color to define edges without adding weight.

## Shapes

The shape language is "Sophisticated Geometry." While corners are rounded to maintain a modern, friendly feel, the radius is kept moderate (0.5rem) to preserve a sense of precision and structure.

- **Standard Containers:** Use `rounded-lg` (1rem) for most glassy cards.
- **Interactive Elements:** Buttons use `rounded-xl` (1.5rem) or full pill shapes to distinguish them from structural containers.
- **Decorative Elements:** Use perfectly circular or 45-degree angled accents to lean into the futurist motif.

## Components

### Glassy Cards
The primary container for projects. Must include:
- Background: `rgba(255, 255, 255, 0.05)`
- Backdrop-filter: `blur(16px)`
- Border: `1px solid rgba(255, 255, 255, 0.1)`
- Subtle top-down linear gradient for the border to mimic light hitting the top edge.

### Action Buttons
Primary buttons use a solid-to-transparent gradient of Primary and Secondary colors. Secondary buttons use a "ghost" style with a primary-colored border and a hover state that fills with a 10% opacity glow.

### Tech Chips
Small, `label-caps` typography tags used for tech stacks (e.g., React, TypeScript). They should have a dark, semi-transparent background and a thin border matching the accent color.

### Interactive Inputs
Input fields are minimal—only a bottom border in neutral slate, which transitions to a full-width primary cyan glow upon focus.

### Project Grid
A staggered or standard 12-column grid displaying cards. Each card should have a "hover lift" effect where the blur intensity increases and the border brightness doubles.

### Navigation
A floating, blurred header that stays fixed at the top. Use `backdrop-filter` to ensure readability as it scrolls over content.