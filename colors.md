# Colors

Two brand colors, navy and green, used together with white. Navy carries the brand; green is the
accent and stands for success: the rising line in the logo.

## Palette

| | Name | HEX | RGB | CMYK (approx.) | Role |
|---|---|---|---|---|---|
| ![Navy](swatches/navy.svg) | **Navy** | `#141452` | 20, 20, 82 | 76, 76, 0, 68 | Primary. Logo, headings, dark backgrounds. |
| ![Green](swatches/green.svg) | **Green** | `#45B945` | 69, 185, 69 | 63, 0, 63, 27 | Accent. Success, progress, highlights. Use sparingly. |
| ![White](swatches/white.svg) | **White** | `#FFFFFF` | 255, 255, 255 | 0, 0, 0, 0 | Backgrounds and text on navy. |
| ![Black](swatches/black.svg) | **Black** | `#000000` | 0, 0, 0 | 0, 0, 0, 100 | Black-only print. Not part of the screen palette. |

The CMYK values are converted from RGB, not matched to a print standard. Ask your printer for a
proof before a large run. No Pantone references have been defined.

## Using the colors

- **Navy and white do most of the work.** Use navy for text, headings and dark surfaces, white for
  backgrounds and for text on navy.
- **Green is an accent, not a background color for text.** Use it for the logo's rising line,
  success states, progress, icons and small highlights.
- **On navy, green works for text and icons;** on white, use it only for graphics and large shapes
  (see contrast below).
- Don't introduce tints, gradients or other colors into the logo. The logo files come in fixed
  versions; see [`callmaker-dialer/`](callmaker-dialer/).

## Contrast

WCAG 2 contrast ratios between the brand colors:

| Foreground on background | Ratio | Body text (4.5:1) | Large text (3:1) |
|---|---|---|---|
| Navy on white | 16.8 : 1 | Pass | Pass |
| White on navy | 16.8 : 1 | Pass | Pass |
| Green on navy | 6.6 : 1 | Pass | Pass |
| Green on black | 8.3 : 1 | Pass | Pass |
| Green on white | 2.5 : 1 | **Fail** | **Fail** |

Green on white is too light for text or for interface elements that must be seen, such as icons
and borders. The green line in the logo is exempt: logos have no contrast requirement, and the
navy parts carry the logo on light backgrounds.

## For developers

```css
:root {
  --brand-navy: #141452;
  --brand-green: #45b945;
  --brand-white: #ffffff;
}
```
