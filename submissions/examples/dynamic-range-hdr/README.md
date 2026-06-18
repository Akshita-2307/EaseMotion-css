# CSS Dynamic Range HDR Demo

## Overview
Demonstrates using `@media (dynamic-range: high)` to detect HDR-capable displays and serve enhanced wide-gamut colors using `oklch()` and `color(display-p3)` while providing graceful SDR fallbacks.

## Features
- **`@media (dynamic-range: high)`** — detects displays with high dynamic range capability
- **`color-gamut`** — detects P3 or sRGB color space support
- **`oklch()` colors** — perceptually uniform color space with wide gamut
- **`color(display-p3)`** — Display P3 color space for in-gamut HDR colors
- **Graceful degradation** — SDR displays receive sRGB-safe fallback colors

## How to Use
1. Define base colors in `oklch()` for all displays
2. Wrap HDR-enhanced versions inside `@media (dynamic-range: high)`
3. Optionally use `@supports (color: color(display-p3 1 0 0))` for P3 support
4. Add glow/shadow effects for HDR to take advantage of the higher luminance range
