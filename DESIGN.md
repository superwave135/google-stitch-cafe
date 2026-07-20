---
name: Fig & Filter
colors:
  surface: '#fff8f8'
  surface-dim: '#e1d8d9'
  surface-bright: '#fff8f8'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#fbf1f2'
  surface-container: '#f5eced'
  surface-container-high: '#efe6e7'
  surface-container-highest: '#e9e0e1'
  on-surface: '#1e1b1c'
  on-surface-variant: '#4d444b'
  inverse-surface: '#342f30'
  inverse-on-surface: '#f8eeef'
  outline: '#7e747c'
  outline-variant: '#cfc3cc'
  surface-tint: '#755377'
  primary: '#331736'
  on-primary: '#ffffff'
  primary-container: '#4a2c4d'
  on-primary-container: '#ba94bb'
  inverse-primary: '#e3b9e3'
  secondary: '#7d5700'
  on-secondary: '#ffffff'
  secondary-container: '#ffc55f'
  on-secondary-container: '#755100'
  tertiary: '#1b2500'
  on-tertiary: '#ffffff'
  tertiary-container: '#303b0f'
  on-tertiary-container: '#98a66f'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffd6fe'
  primary-fixed-dim: '#e3b9e3'
  on-primary-fixed: '#2c1030'
  on-primary-fixed-variant: '#5b3c5e'
  secondary-fixed: '#ffdeaa'
  secondary-fixed-dim: '#f5bd58'
  on-secondary-fixed: '#271900'
  on-secondary-fixed-variant: '#5f4100'
  tertiary-fixed: '#dbe9ac'
  tertiary-fixed-dim: '#bfcd92'
  on-tertiary-fixed: '#161f00'
  on-tertiary-fixed-variant: '#404b1e'
  background: '#fff8f8'
  on-background: '#1e1b1c'
  surface-variant: '#e9e0e1'
  fig-purple: '#4A2C4D'
  amber-accent: '#D9A441'
  paper-bg: '#FAF6F0'
  ink-black: '#221E1F'
typography:
  display-lg:
    fontFamily: Libre Caslon Text
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Libre Caslon Text
    fontSize: 36px
    fontWeight: '700'
    lineHeight: '1.1'
  headline-md:
    fontFamily: Libre Caslon Text
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-sm:
    fontFamily: Libre Caslon Text
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-caps:
    fontFamily: Hanken Grotesk
    fontSize: 14px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.05em
  price-tag:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '600'
    lineHeight: '1'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1100px
  gutter: 24px
  margin-mobile: 20px
  margin-desktop: 40px
  stack-sm: 8px
  stack-md: 24px
  stack-lg: 48px
  section-gap: 80px
---

## Brand & Style

The design system is built for a neighborhood staple that balances the artisanal precision of a roastery with the unpretentious warmth of a local café. The visual language is **Corporate / Modern** with a **Tactile** edge—it avoids "coffee shop" clichés (distressed woods, chalkboards) in favor of a clean, structured, and editorial aesthetic that feels both professional and approachable.

The personality is "dry-humored and plainspoken." This is achieved through a layout that values high-contrast clarity and generous whitespace, allowing the characterful typography and high-quality photography to do the heavy lifting. The UI remains humble and invisible, ensuring the user's journey—whether finding the address or ordering catering—is friction-less and direct.

The emotional response should be one of reliability and understated quality. It feels "Roasted here. Baked here." because the design itself looks intentional and handcrafted, yet efficient.

## Colors

The palette is rooted in a "paper and ink" philosophy. The **paper-bg (#FAF6F0)** provides a warm, organic foundation that is easier on the eyes than pure white, while **ink-black (#221E1F)** provides sharp, high-contrast legibility for all body copy.

**Primary Fig Purple (#4A2C4D)** is used for structural elements, headers, and primary brand touchpoints. It represents the depth of the coffee roast and the maturity of the business. 

**Amber-Accent (#D9A441)** is strictly reserved for interactive UI elements (buttons, active states, markers). It must never be used for body text to ensure WCAG accessibility and brand discipline. This color acts as a "highlight," guiding the user's eye to the one primary call-to-action on each page.

## Typography

This design system employs a classic pairing of a "characterful" serif and a "clean" sans-serif. 

**Libre Caslon Text** is used for all headlines. Its literary heritage reinforces the "roastery" aspect—suggesting craft and history. It should be set with tight leading and slight negative letter-spacing at large sizes for a modern, editorial feel.

**Hanken Grotesk** is used for body text and functional labels. It is a highly legible, contemporary sans-serif that stays out of the way. All body text should be set in `ink-black` for maximum readability. For price lists, use `tabular-nums` to ensure that prices align vertically in menus.

Mobile-specific overrides are provided for the largest display sizes to ensure they do not wrap awkwardly on small devices.

## Layout & Spacing

This design system uses a **Fluid Grid** with a strict mobile-first implementation. On mobile, all content is confined to a single column with 20px side margins. On desktop, the layout expands to a maximum width of 1100px, utilizing a 12-column grid.

Spacing follows an 8px base unit. 
- **Vertical Rhythm:** Sections are separated by large gaps (`section-gap`) to give the content room to breathe, reflecting the "stay as long as you like" café philosophy. 
- **Menu Layout:** On mobile, menu items are stacked. On desktop, they reflow into a 2-column grid.
- **Catering Cards:** These stack vertically on mobile and sit in a 3-column row on desktop for easy comparison.

The "Visit" page must prioritize information density at the top (the "fold") to ensure address and hours are visible immediately upon load without scrolling.

## Elevation & Depth

To maintain the "plainspoken" brand voice, this design system avoids heavy shadows or complex gradients. 

**Depth is conveyed through Tonal Layers:**
- The primary surface is `paper-bg`. 
- Overlays or modal-like sections use `ink-black` with white text for a high-contrast "pop."
- **Low-contrast outlines:** Cards (like those in the Catering section) should use a subtle 1px border of `fig-purple` at 15% opacity or a slightly darker shade of the background color rather than a shadow.

When a shadow is absolutely necessary for interactive clarity, use a **Hard Shadow**: a 2px offset with 100% opacity in `fig-purple` or `ink-black`, creating a "sticker" or "cut-out" effect rather than a soft ambient glow.

## Shapes

The shape language is **Soft (0.25rem)**. This slight rounding takes the edge off the "brutalist" layout, making the interface feel approachable and friendly without becoming "bubbly" or juvenile. 

- **Images:** Should be kept sharp (0px radius) or use the same soft 4px radius to feel like printed photographs.
- **Buttons & Inputs:** Use the standard `rounded` (4px) setting.
- **Dietary Markers (V, VG, GF):** These can be treated as circular pills to differentiate them from actionable UI buttons.

## Components

### Buttons
- **Primary:** Background `amber-accent`, text `ink-black`, 700 weight. High visibility. Only one per page.
- **Secondary/Link:** Text `ink-black`, underlined, or with a simple trailing arrow. No background fill.
- **Footer Link:** `paper-bg` text on `ink-black` background.

### Cards (Catering/Packages)
A card consists of a 1px `fig-purple` (low opacity) border, a `headline-sm` title, a price in `price-tag` style, and a list of inclusions. The primary button is always anchored to the bottom.

### Input Fields (Contact/Enquiry)
Clean, bottom-border only or a light 1px stroke. Labels are `label-caps`. Focus state uses a 2px `amber-accent` bottom border.

### Menu Items
A list-based component. Item name (left, `body-md` bold), price (right, `price-tag`), and description (below, `body-md` muted). Dietary markers follow the item name in a small, circular pill.

### Navigation
Simple text links in `label-caps`. On mobile, use a clean "Menu" label or a simple list—avoid overly complex hamburger animations. The navigation should feel like a simple table of contents.