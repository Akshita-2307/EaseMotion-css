# CSS transition-behavior: allow-discrete

## What does this do?
Demonstrates animating discrete CSS properties (like `display` and `overlay`) using `transition-behavior: allow-discrete` combined with `@starting-style` for smooth entry and exit animations.

## How is it used?
Add the classes to any HTML element:

    <div class="discrete-card">Content</div>
    <div class="popover-trigger" popover>Popover content</div>

## Why is it useful?
Before `transition-behavior: allow-discrete`, discrete properties like `display` could not be animated, causing abrupt show/hide transitions. This feature enables smooth opening and closing animations for popovers, dialogs, and conditional UI elements.

## Tech Stack
- HTML
- CSS (no frameworks, no JavaScript)

## Preview
Open demo.html directly in your browser to see the effect.

## Contribution Notes
- Class naming was handled by the contributor
- Maintainer will rename to ease-* convention before merging
