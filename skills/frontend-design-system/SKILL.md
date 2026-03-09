---
name: frontend-design-system
description: Generates refined, distinctive frontend UI designs. Use when creating landing pages, dashboards, web applications, or UI components. Avoids generic "AI slop" aesthetics in favour of professional, memorable interfaces.
---

# Frontend Design System

## Overview

This skill provides guidelines for creating polished, distinctive frontend UIs that avoid the generic, characterless aesthetics that AI-generated interfaces tend to produce.

## Anti-Patterns

The following patterns produce what is known as "AI slop aesthetics" — avoid them:

### Typography

- ❌ Overused fonts: Inter, Roboto, Open Sans
- ❌ The same font family for all text
- ❌ Only standard font weights

### Colors

- ❌ Purple-to-pink gradients
- ❌ Generic blue or green accent colors
- ❌ Oversaturated neon colors
- ❌ Default Tailwind color palette used as-is

### Layout

- ❌ Standard hero section: text left, image right (50/50 split)
- ❌ Three-column equal-width feature grids
- ❌ Centre-aligned uniform card layouts

### Effects

- ❌ Excessive blur effects
- ❌ Animations applied to every element
- ❌ Overused glassmorphism

## Best Practices

### Typography

**Recommended font pairings:**

| Heading          | Body            | Character                    |
| ---------------- | --------------- | ---------------------------- |
| Playfair Display | Source Sans Pro | Classic meets modern         |
| Space Grotesk    | Inter           | Tech, minimal                |
| Fraunces         | Work Sans       | Elegant, highly readable     |
| DM Serif Display | DM Sans         | Cohesive contrast            |
| Syne             | Outfit          | Bold, contemporary           |

**Typography principles:**

- Use different font families for headings and body (pair serif with sans-serif)
- Leverage font weight variation (300, 400, 600, 800)
- Use letter-spacing to create visual hierarchy

### Colors

**Palette construction:**

```
Primary:   The brand's main identity color
Secondary: Complements the primary (complementary or analogous)
Accent:    A high-attention color for CTAs and highlights
Neutral:   Greys for backgrounds and body text
```

**Techniques for distinctiveness:**

- Use HSL adjustments to introduce subtle hue shifts
- In dark mode: reduce saturation, adjust lightness rather than just inverting
- Customise semantic colors (success, warning, error) to match the brand

### Layout

**Differentiating layout patterns:**

- Asymmetric grids (5:7 or 2:3 ratios)
- Overlapping elements with negative margins
- Diagonal section dividers
- Bento grids and organic arrangements
- Bold use of whitespace

### Animation & Motion

**Effective animation principles:**

1. **Focus on high-impact moments**
   - A single, well-timed animation on page load
   - Immediate feedback on user actions (click, hover)
   - Visual representation of state changes (success, error)

2. **Timing guidelines**
   - Micro-interactions: 150–300ms
   - Page transitions: 300–500ms
   - Complex animations: 500–800ms

3. **Easing functions**
   ```css
   --ease-out-expo:     cubic-bezier(0.16, 1, 0.3, 1);
   --ease-out-quart:    cubic-bezier(0.25, 1, 0.5, 1);
   --ease-in-out-quart: cubic-bezier(0.76, 0, 0.24, 1);
   ```

### Background & Texture

**Background design ideas:**

- Subtle noise texture
- Geometric patterns (used sparingly)
- Gradient mesh
- Abstract blobs / shapes
- Parallax background layers

## Implementation Checklist

- [ ] Typography: select distinct heading and body fonts
- [ ] Color palette: build a cohesive palette of 5+ colors
- [ ] Layout: consider an asymmetric or non-standard grid system
- [ ] Animation: implement 1–2 high-impact animations
- [ ] Background: add a texture or distinctive background element
- [ ] Consistency: verify all elements conform to the design system

## Theme Examples

For detailed theme implementations see:

- [Theme examples](themes.md)
- [Component reference](components.md)

## Quick Reference

**Font pairing cheat sheet:**

1. Modern & clean → Space Grotesk + Inter
2. Elegant & premium → Playfair Display + Lato
3. Tech startup → Syne + Outfit
4. Warm & approachable → Fraunces + Work Sans
5. Bold & creative → DM Serif Display + DM Sans

**Color resources:**

- Coolors.co — generate harmonious palettes
- Realtime Colors — live preview
- Happy Hues — inspiration
