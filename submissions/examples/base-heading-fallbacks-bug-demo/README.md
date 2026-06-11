# base.css: Headings use var() without fallback values

**Issue:** #5951
**File:** `core/base.css`

## Problem

Lines 38, 41-46 use `var(--ease-color-neutral-900)`, `var(--ease-text-4xl)`, etc without fallback values for heading typography tokens.

## Expected

```css
h1 { font-size: var(--ease-text-4xl, 2.25rem); }
h2 { font-size: var(--ease-text-3xl, 1.875rem); }
```

## Demo

Open `demo.html` without the variables layer to see headings with zero/initial font-size.
