# Masonry: Reduced-motion rule kills transitions on ALL children

**Issue:** #5949
**File:** `components/masonry.css`

## Problem

Lines 217-222 apply `transition: none !important` to ALL `.ease-masonry > *` children under `prefers-reduced-motion`, not just animated elements. This is overly broad and prevents intentional transitions from working.

## Expected

Only target elements that have transitions, or use a more specific selector.

## Demo

Open `demo.html` and enable reduced motion to see all transitions killed on masonry children.
