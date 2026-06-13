# Modal Backdrop Token

Demonstrates a bug where the modal backdrop overlay uses a hardcoded color value instead of the framework's `--ease-overlay` token, making it inconsistent with the design token system.

**Issue:** [#5758 — Modal backdrop token](https://github.com/anomalyco/easemotion/issues/5758)

---

## What does this show?

The modal backdrop (semi-transparent overlay behind modals) uses `background: rgba(0,0,0,0.5)` directly instead of `var(--ease-overlay-bg, rgba(0,0,0,0.5))`. Users cannot customize the backdrop via CSS variables.

---

## Files

| File | Purpose |
|------|---------|
| `demo.html` | Compares hardcoded vs token-based backdrop |
| `style.css` | Modal backdrop styles with and without tokens |
| `README.md` | This file |
