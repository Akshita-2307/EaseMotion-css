# Validate Bundle Empty

Demonstrates a bug where the build validation script returns a false-positive success when the generated CSS bundle is empty.

**Issue:** [#5759 — Validate bundle empty](https://github.com/anomalyco/easemotion/issues/5759)

---

## What does this show?

When the build pipeline produces an empty `easemotion.min.css` (e.g. due to a build error or missing imports), the validation step passes without warning. An empty bundle silently breaks all framework styles in production.

---

## Files

| File | Purpose |
|------|---------|
| `demo.html` | Shows the difference between valid and empty bundle loading |
| `style.css` | Styles demonstrating bundle validation |
| `README.md` | This file |
