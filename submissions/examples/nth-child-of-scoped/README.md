# CSS :nth-child(an+b of .scoped)

## What does this do?

Demonstrates the `:nth-child(an+b of <selector>)` syntax — scoped structural selectors that match elements based on their position *among siblings matching a filter selector*, not among all siblings.

## How is it used?

```css
/* Style the 2nd, 4th, 6th… visible item */
.item:nth-child(2n of .visible) {
  background: var(--accent);
}
```

Without the `of .visible` clause, `:nth-child(2n)` would target every even child regardless of class. With scoping, only `.visible` elements are counted.

## Why is it useful?

Before this syntax, filtering sibling subsets required JavaScript to recalculate indices and apply classes. With `:nth-child(an+b of <selector>)`, the browser handles the filtering natively — cleaner markup, no JS bookkeeping, and declarative styling of filtered lists, grids, and tables.
