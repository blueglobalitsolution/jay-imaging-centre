# Design System Inspired by Home

> Auto-extracted from `https://hospitalia.framer.website/` on 2026-07-14

## 1. Visual Theme & Atmosphere

Friendly, approachable design with rounded shapes and generous whitespace.

The hero section leads with "quality & expert care for your health".

**Key Characteristics:**
- Poppins as the heading font (custom web font loaded via @font-face)
- sans-serif as the body font for all running text
- Heading weight 700, letter-spacing -2.4px
- Light/white background (#ffffff) as the primary canvas
- Primary accent `#257eeb` used for CTAs and brand highlights
- 5 shadow level(s) detected — tinted shadows
- Rounded corners (16px+) creating a friendly, approachable feel
- Tags: light, rounded, accented, sans-serif

## 2. Color Palette & Roles

### Primary
- **Primary Accent** (`#257eeb`) · `--color-primary`: Brand color, CTA backgrounds, link text, interactive highlights.
- **Background** (`#ffffff`) · `--color-bg`: Page background, primary canvas.
- **Background Secondary** (`#257eeb`) · `--color-bg-secondary`: Cards, surfaces, alternating sections.

### Text
- **Text Primary** (`#000000`) · `--color-text`: Headings and body text.
- **Text Secondary** (`#505f62`) · `--color-text-secondary`: Muted text, captions, placeholders.

### Borders & Surfaces
- **Border** (`#eff6ff`) · `--color-border`: Dividers, outlines, input borders.

### Full Extracted Palette

| # | Hex | CSS Variable | Role | Area | Contrast |
|---|---|---|---|---|---|
| 1 | `#ffffff` | `--palette-1` | block | large | text-dark |
| 2 | `#257eeb` | `--palette-2` | text-accent | large | text-light |
| 3 | `#eff6ff` | `--palette-3` | button | large | text-dark |
| 4 | `#505f62` | `--palette-4` | badge | medium | text-light |
| 5 | `#0000ee` | `--palette-5` | text-accent | medium | text-light |
| 6 | `#173254` | `--palette-6` | text-accent | small | text-light |
| 7 | `#47576b` | `--palette-7` | text-accent | small | text-light |

## 3. Typography Rules

- **Heading Font:** `Poppins` (web font)
- **Body Font:** `sans-serif`, sans-serif

### Type Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing |
|---|---|---|---|---|---|
| H1 | Poppins | 60px | 700 | 81px | -2.4px |
| H2 | Poppins | 44px | 700 | 59.4px | normal |
| H3 | Poppins | 24px | 700 | 32.4px | normal |
| Body | Poppins | 18px | 500 | 22.5px | 1px |

### Type Scale

| Token | Size | Suggested Usage |
|---|---|---|
| Display | `60px` | headings |
| H1 | `44px` | headings |
| H2 | `24px` | headings |
| H3 | `20px` | headings |
| H4 | `18px` | headings |
| Body L | `16px` | body / supporting text |
| Body | `14px` | body / supporting text |
| Small | `12px` | body / supporting text |

## 4. Component Stylings

No prominent button or card components detected. Use the color palette and typography rules above to create components consistent with the brand.

## 5. Layout Principles

- **Base spacing unit:** `24px` — use multiples (48px, 72px, 96px, etc.)

### Spacing Scale (extracted from real elements)

| Token | Value | Role |
|---|---|---|
| spacing-1 | `24px` | card |
| spacing-2 | `12px` | element |
| spacing-3 | `16px` | element |
| spacing-4 | `32px` | card |
| spacing-5 | `8px` | element |
| spacing-6 | `100px` | section |
| spacing-7 | `48px` | card |
| spacing-8 | `60px` | section |

### Border Radius Scale

| Token | Value | Element |
|---|---|---|
| radius-card | `16px` | card |
| radius-pill | `100px` | pill |
| radius-card | `50px` | card |
| radius-subtle | `4px` | subtle |
| radius-card | `24px` | card |
| radius-card | `32px` | card |

## 6. Depth & Elevation

| Level | Shadow | Usage |
|---|---|---|
| High | `rgba(71, 87, 107, 0.15) 0px 0px 15px 0px` | Modals, floating elements |
| Mid | `rgba(80, 95, 98, 0.1) 0px 0px 10px 0px` | Dropdowns, popovers |
| High | `rgba(0, 0, 0, 0.15) 0px 0px 15px 0px` | Modals, floating elements |
| Low | `rgba(71, 87, 107, 0.15) 0px 0px 0px 0px` | Cards, subtle elevation |
| Low | `rgba(0, 0, 0, 0.26) 0px 0.636953px 1.14652px -1.125px, rgba(0, 0, 0, 0.24) 0px 1...` | Cards, subtle elevation |

> **Note:** This site uses chromatic (color-tinted) shadows rather than pure black — this is a deliberate brand choice that adds warmth to elevation.

## 7. Do's and Don'ts

### Do
- Use `#ffffff` as the primary background color
- Use `Poppins` for all headings and `sans-serif` for body text
- Use `#257eeb` as the single dominant accent/CTA color
- Maintain `24px` as the base spacing unit — all gaps should be multiples
- Use rounded corners (`16px`+) consistently for all interactive elements
- Apply the shadow system for elevation — use the extracted shadow values
- Use weight 700 for headings to match the brand's typographic voice

### Don't
- Don't use colors outside the extracted palette without justification
- Don't substitute Poppins/sans-serif with generic alternatives
- Don't use irregular spacing — stick to 24px grid
- Don't use dark/black backgrounds — this is a light-themed design
- Don't use sharp corners — they feel hostile in this rounded design language
- Don't use pure black (#000000) for text — use `#000000` instead
- Don't add decorative elements not present in the original design — no badges, ribbons, banners, or ornaments unless the source site uses them
- Don't invent UI patterns the source site doesn't have — if the original has no NEW badge, don't add one just because a red is in the palette

## 8. Responsive Behavior

| Breakpoint | Width | Notes |
|---|---|---|
| Mobile | < 640px | Single column, stack sections, reduce font sizes ~80% |
| Tablet | 640–1024px | 2-column where appropriate, maintain spacing ratios |
| Desktop | 1024–1440px | Full layout as designed |
| Wide | > 1440px | Max-width container, center content |

- Touch targets: minimum 44×44px on mobile
- Maintain 24px base unit across breakpoints — only scale multipliers

## 9. Agent Prompt Guide

### Quick Color Reference

```
Background:  #ffffff
Text:        #000000
Accent:      #257eeb
Border:      #eff6ff
```

### Example Prompts

1. "Build a hero section with a `#ffffff` background, `Poppins` heading in `#000000`, and a `#257eeb` CTA button."
2. "Create a pricing card using background `#257eeb`, border `#eff6ff`, `sans-serif` for text, and 72px padding."
3. "Design a navigation bar — `#ffffff` background, `#000000` links, `#257eeb` for active state."
4. "Build a feature grid with 3 columns, 72px gap, each card using the card component style."
5. "Create a footer with `#000000` background, `#ffffff` text, and 48px padding."

### Iteration Guide

1. Start with layout structure (sections, grid, spacing)
2. Apply colors from the palette — background first, then text, then accents
3. Set typography — font families, sizes from the type scale, weights
4. Add components — buttons, cards, inputs using the specs above
5. Apply border-radius consistently across all elements
6. Add shadows for depth — use the extracted shadow values, not defaults
7. Check responsive behavior — test mobile and tablet layouts
8. Final pass — verify all colors match, spacing is consistent, fonts are correct
