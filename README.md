# Nautical Dusk — Professional Website

A portfolio and professional presence site built on the **Nautical Dusk** design system — a maritime-inspired aesthetic centered on the concept of *stillness in motion*, using an albatross motif against layered atmospheric backgrounds.

**Live site:** https://www.mariosalinas.com
**Author:** Mario Salinas  
**GitHub:** [mojave-ghost](https://github.com/mojave-ghost)

---

## Overview

This is a single-page professional website featuring editorial typography, cinematic color banding, and a restrained accent palette drawn from a dusk ocean scene. The site serves as a portfolio, about page, and contact point.

### Sections

- **Navigation** — Sticky nav with Cormorant Garamond brand name, Inter all-caps links, and Horizon Glow active indicator
- **Hero** — Full-viewport section with horizontal color banding, film grain overlay, albatross SVG silhouette, and ghost button CTAs
- **About** — Dark textured section with a 7/5 column split, headshot with duotone treatment, and editorial copy
- **Projects** — Three-column card grid on an Open Ocean surface, each card with a Horizon Glow left border accent
- **Pull Quote** — Centered blockquote in Cormorant Garamond with a Dusk Bloom opening quotation mark
- **Services** — Light Sea Foam section with white service cards and an orange left-border rule
- **Footer** — Four-column layout with bird mark, navigation links, contact info, and availability status

## Design System

The site follows the Nautical Dusk Design System v1.0 (February 2026). Key tokens:

| Token | Value | Role |
|---|---|---|
| Night Water | `#1A2B45` | Primary dark surface |
| Open Ocean | `#2E4A72` | Card surfaces on dark backgrounds |
| Horizon Glow | `#E8713A` | Accent — CTAs, rules, active states |
| Dusk Bloom | `#E8A0A8` | Accent — quote marks, tags, labels |
| Storm Slate | `#4A5568` | Neutral mid-tone |
| Sea Foam | `#F7F5F2` | Light background sections |
| Salt | `#FFFFFF` | Text on dark surfaces only |

### Typography

- **Headings:** Cormorant Garamond, weight 300, 52–72px (H1) fluid scaling
- **Body:** Inter, weight 400, 16–18px, line-height 1.7, max-width 680px
- **Labels/Nav:** Inter, weight 500, all caps, 0.08em letter-spacing

### Design Rules

- No drop shadows — depth is communicated through border thickness
- The albatross silhouette is always flat, single-color, and still — never animated or gradient-filled
- Film grain is applied via CSS SVG `feTurbulence` filter as a pseudo-element
- Background atmosphere uses horizontal color banding (4–6 bands), not continuous gradients
- Section alternation follows a dark → light → dark rhythm
- Horizon Glow never fills large areas — it is the light, not the sky

## Project Structure

```
my-professional-website/
├── index.html              # Production site (single-file, self-contained)
├── README.md               # This file
├── nauticalduskdesigndoc.pdf   # Full design system specification
├── nautical-dusk-lowfidelity-wireframes.html  # Annotated wireframes (9 frames)
└── IMG_4778.jpg            # Headshot (About section)
```

## Tech Stack

- **HTML/CSS** — Single-file, framework-agnostic, no build step
- **Fonts** — Google Fonts (Cormorant Garamond, Inter)
- **Icons** — Phosphor Icons, thin weight
- **Layout** — CSS Grid, 12-column with 24px gutters, max-width 1280px
- **Responsive** — Mobile-first with breakpoints at 576px, 768px, and 1280px

## Responsive Behavior

| Breakpoint | Grid | Nav | Projects | Hero Layout |
|---|---|---|---|---|
| < 576px | 4-col, 16px gutter | Brand + ghost CTA only | 1 column | Single column, bird centered |
| 576–767px | 8-col, 20px gutter | Brand + ghost CTA only | 2 columns | Single column, bird centered |
| ≥ 768px | 12-col, 24px gutter | Full nav links visible | 3 columns | 7/5 split, bird right-weighted |

## Running Locally

No build tools required. Open `index.html` in a browser:

```bash
# Clone the repository
git clone https://github.com/mojave-ghost/my-professional-website.git
cd my-professional-website

# Open in default browser (macOS)
open index.html

# Or serve locally
python3 -m http.server 8000
```

## Design Artifacts

The `/` directory includes design process artifacts:

- **`nauticalduskdesigndoc.pdf`** — The complete design system document covering color, typography, imagery rules, UI components, layout specs, content voice, and implementation notes
- **`nautical-dusk-lowfidelity-wireframes.html`** — Nine annotated wireframe frames covering navigation, hero, dark/light content sections, cards, pull quote, footer, mobile breakpoint, and a component reference sheet

## License

© 2026 Mario Salinas. All rights reserved.
