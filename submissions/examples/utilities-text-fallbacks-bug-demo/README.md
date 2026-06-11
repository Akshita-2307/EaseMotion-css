# Utilities: Text size utilities missing var() fallback values

**Issue:** #5959
**File:** `core/utilities.css`

## Problem

Lines 250-257 define `.ease-text-xs` through `.ease-text-4xl` using `var(--ease-text-xs)` through `var(--ease-text-4xl)` without any fallback values.

## Expected

```css
.ease-text-xs   { font-size: var(--ease-text-xs, 0.75rem) !important; }
.ease-text-sm   { font-size: var(--ease-text-sm, 0.875rem) !important; }
.ease-text-base { font-size: var(--ease-text-base, 1rem) !important; }
```

## Demo

Open `demo.html` to see text size utilities resolve to `initial` without the base layer.
