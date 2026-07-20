# Fig & Filter

A five-page static website for **Fig & Filter**, a neighborhood café, roastery, and bakehouse. This website balances the artisanal precision of a roastery with the unpretentious warmth of a local café, implementing a clean, structured, and editorial design system.

---

## 📖 Table of Contents
1. [Project Overview](#project-overview)
2. [Design System & Styling](#design-system--styling)
3. [Page Structure](#page-structure)
4. [Accessibility & Best Practices](#accessibility--best-practices)
5. [Directory Layout](#directory-layout)
6. [Local Development](#local-development)

---

## Project Overview

The website is a five-page static web application built using **plain HTML, CSS, and lightweight JavaScript** strictly for the responsive mobile navigation toggle. All copy and images are populated verbatim from the project's content assets without modifications, ensuring a dry-humored, plainspoken brand voice.

### Key Guidelines Followed
- **No external assets**: Images are bundled locally and referenced via relative paths.
- **Copy fidelity**: The content of all pages matches the content manifest files word for word.
- **Strict single-CTA design**: Every page contains exactly one primary visual call to action (accented button).

---

## Design System & Styling

The visual language follows the specs in [DESIGN.md](file:///home/geekytan/Documents/ntu_dsai/google-stitch-design/DESIGN.md):
- **Colors**:
  - **Surface/Background**: Warm off-white (`#FAF6F0`) representing "paper."
  - **Body text**: Near-black (`#221E1F`) for high-contrast legibility.
  - **Primary Brand**: Fig purple (`#4A2C4D`) for structural elements and headers.
  - **Accent**: Warm amber (`#D9A441`) strictly reserved for the single primary call-to-action (CTA) button or active visual markers.
- **Typography**:
  - **Headings**: `Libre Caslon Text` (serif) set with tight leading and negative letter-spacing for editorial feel.
  - **Body text**: `Hanken Grotesk` (clean sans-serif) for high legibility, minimum size `16px`.
- **Spacing**:
  - Based on an **8px base unit**.
  - **Vertical Rhythm**: Section gaps set to `80px` to let the content breathe.
  - **Fluid Grid**: Mobile-first single column expanding to a maximum of `1100px` on desktop with `40px` margins.
- **Borders & Corners**:
  - Soft rounding (`4px` / `0.25rem` radius) on buttons, cards, and inputs.
  - Hard shadows (2px offset with 100% opacity in `fig-purple` or `ink-black`) when needed for interactive pop.

---

## Page Structure

The website consists of the following 5 pages sharing a single [styles.css](file:///home/geekytan/Documents/ntu_dsai/google-stitch-design/styles.css):

### 1. Home (`index.html`)
- **Job**: Convince a stranger to walk in.
- **Key Elements**: Full-width header showing espresso pour, essentials banner (hours, address, and primary "Find us" CTA), three reasons to visit, and a secondary link to the Menu.

### 2. Menu (`menu.html`)
- **Job**: Let a visitor find what they want to order in under a minute.
- **Key Elements**: Structured list of Coffee, Not Coffee, All-Day Kitchen, and Bakery items with tabular prices, dietary markers (V, VG, GF), and illustrations. Includes an "Order catering" CTA.

### 3. Catering (`catering.html`)
- **Job**: Get an office manager to send a catering enquiry.
- **Key Elements**: Three comparative package cards (The Coffee Run, The Morning Tea, The Full Spread), ordering process details, and the primary "Order catering" email CTA.

### 4. About (`about.html`)
- **Job**: Make the café feel like people, not just a business.
- **Key Elements**: Café founding story, founder profiles for Mara (kitchen) and Dev (coffee) with portrait crop photos, and details of the roasting schedule in a custom tonal card.

### 5. Visit (`visit.html`)
- **Job**: Get someone through the door immediately.
- **Key Elements**: Prioritizes information density at the top (address and hours are visible above the fold on mobile), directions by transit/car, guidelines, and an "Email Us" primary CTA.

---

## Accessibility & Best Practices

- **Touch Targets**: Every link and button is styled with a minimum target height of **44px** to ensure easy tapping on mobile devices.
- **Responsive Layout**: Designed mobile-first. Tested to ensure **no horizontal scrolling** at mobile widths down to **375px**, and navigation links collapse into a clean menu toggle below **768px**.
- **WCAG AA Compliance**: All typography pairings (fig purple or near-black on off-white) pass the AA level for color contrast.
- **Verbatim Alt Text**: Every image includes the exact descriptive alt text assigned by the content manifest.

---

## Directory Layout

```
.
├── content/               # Raw markdown copy and original assets
│   ├── images/            # Original photograph files and images.md manifest
│   ├── about.md
│   ├── brand.md
│   ├── catering.md
│   ├── home.md
│   ├── menu.md
│   └── visit.md
├── design/                # PNG screenshots of visual mockups
├── images/                # Copied local photographs referenced by pages
├── index.html             # Home page
├── menu.html              # Menu page
├── catering.html          # Catering page
├── about.html             # About page
├── visit.html             # Visit page
├── styles.css             # Main stylesheet containing all design tokens
├── DESIGN.md              # Design system guidelines
└── README.md              # Project documentation
```

---

## Local Development

Since the site is built with plain HTML and CSS, it does not require a compilation step.

1. **Viewing Pages**: You can open `index.html` directly in any web browser.
2. **Serving Locally**: To serve the files using a simple HTTP server (for relative paths and script loading consistency):
   ```bash
   # Using Python 3
   python3 -m http.server 8000
   
   # Or using Node.js static server
   npx serve .
   ```
3. Open your browser and navigate to `http://localhost:8000` (or the port specified by the server).
