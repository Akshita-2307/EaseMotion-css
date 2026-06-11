# Buttons: .ease-btn-icon missing size variants (sm, lg)

**Issue:** #5947
**File:** `components/buttons.css`

## Problem

`.ease-btn-icon` has only a single size. Other button variants (`.ease-btn-sm`, `.ease-btn-lg`) exist for text buttons but there is no `.ease-btn-icon-sm` or `.ease-btn-icon-lg`.

## Expected

```css
.ease-btn-icon-sm { padding: var(--ease-space-2, 0.5rem); border-radius: var(--ease-radius-sm, 0.25rem); }
.ease-btn-icon-lg { padding: var(--ease-space-4, 1rem); border-radius: var(--ease-radius-lg, 1rem); }
```

## Demo

Open `demo.html` to see the icon button with no size variants.
