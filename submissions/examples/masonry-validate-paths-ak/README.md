# Masonry Validate Paths

Demonstrates how incorrect/missing path validation in CSS `masonry` layout leads to broken grid rendering when items reference non-existent or malformed grid areas.

**Issue:** [#5756 — Masonry validate paths](https://github.com/anomalyco/easemotion/issues/5756)

---

## What does this show?

Masonry grid items using `grid-area` references that don't match any defined template area fall into a default flow position, breaking the intended masonry arrangement.

### The Problem

When a masonry item references `grid-area: card-4` but the grid template only defines areas up to `card-3`, the item collapses to an unstyled default position.

### The Fix

Validate all `grid-area` references against the defined `grid-template-areas` at build time, or provide fallback positions for unmatched items.

---

## Files

| File | Purpose |
|------|---------|
| `demo.html` | Broken vs fixed masonry path validation |
| `style.css` | Masonry grid styles with validation |
| `README.md` | This file |
