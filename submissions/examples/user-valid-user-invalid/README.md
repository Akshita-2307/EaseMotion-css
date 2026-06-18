# CSS :user-valid / :user-invalid Form Validation

## Overview
Demonstrates the CSS `:user-valid` and `:user-invalid` pseudo-classes for form validation UX. Unlike `:valid`/`:invalid` which apply immediately on page load, these user-interaction pseudo-classes only activate after the user has interacted with a form field.

## Features
- **`:user-valid`** — applies styles when a field is valid AND the user has interacted with it
- **`:user-invalid`** — applies styles when a field is invalid AND the user has interacted with it
- **Shake animation** — draws attention to fields that fail validation after user interaction
- **`:has()` integration** — parent `.form-group` elements detect child field validation state
- **Password requirements** — live feedback on length, number, and uppercase letter requirements

## How to Use
1. Add `:user-valid` and `:user-invalid` to input selectors alongside normal `:focus` styles
2. Use `form:has(:user-invalid)` to style the entire form when any field has user-flagged errors
3. Pair with `:has()` for parent-level validation indicators
4. Add subtle animations (like shake) only on `:user-invalid` to avoid overwhelming users on page load
