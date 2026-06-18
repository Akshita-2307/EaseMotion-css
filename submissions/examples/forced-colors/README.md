# CSS Forced Colors Mode

A practical demonstration of the CSS `forced-colors` media feature and the `forced-color-adjust` property.

## What is Forced Colors Mode?

Forced Colors Mode is a Windows accessibility feature (formerly High Contrast Mode) that replaces a website's colors with a user-selected theme to improve readability. The `@media (forced-colors: active)` media query detects when this mode is active.

## System Color Keywords

When forced colors mode is active, CSS provides system color keywords that map to the user's theme:

| Keyword | Purpose |
|---|---|
| `Canvas` | Page background |
| `CanvasText` | Body text color |
| `LinkText` | Hyperlink text |
| `ButtonText` | Text on buttons |
| `ButtonFace` | Button background |
| `Highlight` | Selected item background |
| `HighlightText` | Selected item text |
| `GrayText` | Disabled text |
| `Field` | Form input background |
| `FieldText` | Form input text |

## The `forced-color-adjust` Property

- `forced-color-adjust: auto` (default) — Colors are automatically adjusted
- `forced-color-adjust: none` — Preserves the author-defined colors (use sparingly)
