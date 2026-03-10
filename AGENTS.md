# Frontend Design System — Agent Guidelines

> **Important:** When implementing any frontend UI, do not rely on training data defaults. Use the principles below and consult the skill files for detail. Generic AI aesthetics are the failure mode to avoid.

## Core Principle

Every UI you generate must be visually distinctive. The standard AI output — Inter font, blue gradients, centered cards, equal-column grids — is a known failure mode called "AI slop aesthetics." These guidelines exist to prevent it.

## Typography

Always pair two font families: a serif or expressive heading font with a clean body font.

| Heading          | Body            | Use for                      |
| ---------------- | --------------- | ---------------------------- |
| Playfair Display | Source Sans Pro | Classic, editorial           |
| Space Grotesk    | Inter           | Tech, minimal                |
| Fraunces         | Work Sans       | Warm, approachable           |
| DM Serif Display | DM Sans         | Cohesive contrast            |
| Syne             | Outfit          | Bold, contemporary           |

Use font weights 300, 400, 600, and 800. Use letter-spacing to build hierarchy.

**Never use a single font family for the entire page.**

## Colors

Build a custom palette. Do not use raw Tailwind defaults.

```
Primary:   Brand identity color
Secondary: Complements primary (analogous or complementary)
Accent:    High-attention color for CTAs and highlights
Neutral:   Greys for backgrounds and body text
```

Avoid: purple-to-pink gradients, generic blue/green accents, oversaturated neons.

## Layout

Break the standard template. Avoid: 50/50 hero splits, 3-column equal grids, centered card stacks.

Instead use:
- Asymmetric grids (35/65, 2:3 ratios)
- Overlapping elements with negative margins
- Diagonal section breaks
- Bento grids
- Bold whitespace

## Animation

Animate selectively. Pick 1–2 high-impact moments only.

- Micro-interactions: 150–300ms
- Page transitions: 300–500ms
- Complex animations: 500–800ms
- Easing: `cubic-bezier(0.16, 1, 0.3, 1)` (ease-out-expo) for most interactions
- Always include `prefers-reduced-motion` handling

## Quick Theme Reference

| Theme              | Heading Font     | Body Font       | Background | Accent        |
| ------------------ | ---------------- | --------------- | ---------- | ------------- |
| Nordic Minimal     | DM Serif Display | DM Sans         | #f7f5f3    | #c17f59       |
| Neon Brutalism     | Space Grotesk    | JetBrains Mono  | #0a0a0a    | #00ff88       |
| Organic Growth     | Fraunces         | Work Sans       | #f5f1eb    | #d4a574       |
| Tech Noir          | Syne             | Outfit          | #0f0f23    | #22d3ee       |
| Editorial Elegance | Playfair Display | Source Serif Pro| #fafafa    | #dc2626       |

## What to Check Before Finishing

- [ ] Two distinct font families used (heading + body)
- [ ] Custom color palette (not raw Tailwind defaults)
- [ ] Layout is not a standard 50/50 or 3-column equal grid
- [ ] At most 1–2 animations, all with `prefers-reduced-motion` support
- [ ] Color contrast meets WCAG AA (4.5:1 minimum for text)
- [ ] All interactive elements have visible focus states

## Detail Files

- Full design guidelines: `skills/frontend-design-system/SKILL.md`
- Theme implementations (CSS variables): `skills/frontend-design-system/themes.md`
- Component patterns (buttons, cards, nav, hero): `skills/frontend-design-system/components.md`
