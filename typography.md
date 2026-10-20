# Typography

Two typefaces: **Urbanist** for the wordmark and display text, **Roboto** for running text and
product interfaces. Both are free under the SIL Open Font License and available from Google Fonts.

## Urbanist: wordmark and display

A geometric sans with a round, single-story "a". It is the typeface of the CallmakerDialer
wordmark and the voice of headings and other short, prominent text.

- **Wordmark:** "Callmaker" in Urbanist SemiBold (600), "Dialer" in Urbanist Light (300), set as
  one word, **CallmakerDialer**, with a small m and no space. The change in weight is what separates
  the two words. Always use the logo files for the wordmark; don't typeset it yourself. See
  [`callmaker-dialer/`](callmaker-dialer/).
- **Headings and display:** Urbanist SemiBold (600). Use Light (300) only at large sizes, for a
  contrasting second line or a subtitle.
- **Avoid** Urbanist for long passages of text and for small sizes in interfaces; use Roboto there.

Download: https://fonts.google.com/specimen/Urbanist

## Roboto: text and interfaces

The typeface of our product interfaces. Use it for body text, captions, tables, forms and anything
read at length or at small sizes.

- **Body text:** Roboto Regular (400).
- **Emphasis and labels:** Roboto Medium (500) or Bold (700).
- Avoid weights below Regular for text smaller than 16 px.

Download: https://fonts.google.com/specimen/Roboto

## Pairing

| Use | Typeface | Weight |
|---|---|---|
| Logo / wordmark | Logo files only | |
| Headings, titles, slide headlines | Urbanist | SemiBold 600 |
| Large subtitles, secondary display lines | Urbanist | Light 300 |
| Body text, interface text | Roboto | Regular 400 |
| Labels, buttons, emphasis | Roboto | Medium 500 / Bold 700 |

Set headings in navy (`#141452`) on white, or in white on navy. See [colors](colors.md).

## Fallbacks

When the brand fonts can't be loaded, such as in email or in documents shared with people who
don't have them installed, use:

- **Instead of Urbanist:** Arial or Helvetica.
- **Instead of Roboto:** Arial, Helvetica or the system font.

In office documents, embed the fonts when sharing, or fall back to Arial.

## For developers

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Urbanist:wght@300;600&family=Roboto:wght@400;500;700&display=swap">
```

```css
:root {
  --font-display: "Urbanist", "Helvetica Neue", Arial, sans-serif;
  --font-text: "Roboto", "Helvetica Neue", Arial, sans-serif;
}
h1, h2, h3 { font-family: var(--font-display); font-weight: 600; }
body { font-family: var(--font-text); font-weight: 400; }
```
