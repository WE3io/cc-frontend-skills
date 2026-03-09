# Theme Examples

This document provides concrete theme implementations and application guidelines.

## 1. Nordic Minimal

**Concept:** Inspired by Scandinavian design — functional beauty and quiet serenity.

```css
:root {
  /* Colors */
  --color-primary: #2d3748; /* Charcoal */
  --color-secondary: #718096; /* Slate */
  --color-accent: #c17f59; /* Terracotta */
  --color-background: #f7f5f3; /* Warm White */
  --color-surface: #ffffff;
  --color-text: #1a202c;
  --color-text-muted: #4a5568;

  /* Typography */
  --font-heading: 'DM Serif Display', serif;
  --font-body: 'DM Sans', sans-serif;

  /* Spacing */
  --space-unit: 8px;
}
```

**Characteristics:**

- Warm white background
- Terracotta accent
- Bold use of whitespace
- Serif heading paired with sans-serif body

---

## 2. Neon Brutalism

**Concept:** Brutalism meets cyberpunk — bold, unapologetic, and rebellious.

```css
:root {
  /* Colors */
  --color-primary: #000000;
  --color-secondary: #ffffff;
  --color-accent: #00ff88; /* Electric Green */
  --color-accent-alt: #ff6b35; /* Safety Orange */
  --color-background: #0a0a0a;
  --color-surface: #1a1a1a;
  --color-text: #ffffff;
  --color-border: #333333;

  /* Typography */
  --font-heading: 'Space Grotesk', sans-serif;
  --font-body: 'JetBrains Mono', monospace;

  /* Effects */
  --shadow-brutal: 4px 4px 0 var(--color-accent);
  --border-brutal: 3px solid var(--color-secondary);
}
```

**Characteristics:**

- High contrast
- Hard shadows (no soft drop shadows)
- Monospace body font
- Heavy borders

---

## 3. Organic Growth

**Concept:** Nature and sustainability — organic shapes and calm, earthy tones.

```css
:root {
  /* Colors */
  --color-primary: #2d4a3e; /* Forest */
  --color-secondary: #8b7355; /* Earth */
  --color-accent: #d4a574; /* Sand */
  --color-background: #f5f1eb; /* Cream */
  --color-surface: #ffffff;
  --color-text: #2c3e2d;
  --color-text-muted: #5d6b5e;

  /* Typography */
  --font-heading: 'Fraunces', serif;
  --font-body: 'Work Sans', sans-serif;

  /* Shapes */
  --radius-organic: 60% 40% 30% 70% / 60% 30% 70% 40%;
}
```

**Characteristics:**

- Earth-tone palette
- Organic blob shapes
- Hand-drawn style accents
- Textured backgrounds

---

## 4. Tech Noir

**Concept:** Dark-mode first — refined and sophisticated with a tech edge.

```css
:root {
  /* Colors */
  --color-primary: #6366f1; /* Indigo */
  --color-secondary: #8b5cf6; /* Violet */
  --color-accent: #22d3ee; /* Cyan */
  --color-background: #0f0f23; /* Deep Navy */
  --color-surface: #1a1a2e;
  --color-surface-elevated: #252542;
  --color-text: #e2e8f0;
  --color-text-muted: #94a3b8;

  /* Typography */
  --font-heading: 'Syne', sans-serif;
  --font-body: 'Outfit', sans-serif;

  /* Effects */
  --glow-primary: 0 0 20px rgba(99, 102, 241, 0.3);
  --gradient-hero: linear-gradient(
    135deg,
    #6366f1 0%,
    #8b5cf6 50%,
    #22d3ee 100%
  );
}
```

**Characteristics:**

- Deep navy background
- Glow-effect accents
- Gradient used as a point of interest, not a background wash
- Modern sans-serif throughout

---

## 5. Editorial Elegance

**Concept:** Magazine-inspired editorial design — refined, authoritative, and typographically rich.

```css
:root {
  /* Colors */
  --color-primary: #1a1a1a;
  --color-secondary: #6b7280;
  --color-accent: #dc2626; /* Editorial Red */
  --color-background: #fafafa;
  --color-surface: #ffffff;
  --color-text: #111827;
  --color-text-muted: #6b7280;

  /* Typography */
  --font-heading: 'Playfair Display', serif;
  --font-body: 'Source Serif Pro', serif;
  --font-accent: 'Libre Baskerville', serif;

  /* Layout */
  --column-width: 65ch;
  --grid-editorial: 1fr 2fr 1fr;
}
```

**Characteristics:**

- Classic serif typography throughout
- Red accent for headings and links
- 65-character column width for optimal readability
- Generous whitespace and line-height

---

## Application Guidelines

### Theme Application Checklist

- [ ] Define all values as CSS custom properties for consistency
- [ ] Account for both dark mode and light mode variants
- [ ] Verify accessibility — minimum contrast ratio of 4.5:1 for text
- [ ] Adjust font sizes responsively across breakpoints
- [ ] Define hover and focus states for all interactive elements
