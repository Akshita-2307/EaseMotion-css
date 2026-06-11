# Utilities: Margin classes missing var() fallback values

**Issue:** #5955
**File:** `core/utilities.css`

## Problem

Lines 165-170 use `var(--ease-space-*)` without fallback values for margin utility classes.

## Expected

Every margin utility should include a fallback, e.g. `margin: var(--ease-space-1, 0.25rem) !important;`.

## Demo

Open `demo.html` to see margin utilities resolve to `initial` without the base layer.
