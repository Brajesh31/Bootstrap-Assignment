# 📱 Responsive Design Guide

## 1. Purpose

All three exercises use Bootstrap 5.3.2 classes, but custom markup and inline styles still need responsive verification. A Bootstrap dependency does not guarantee that every custom layout adapts correctly.

## 2. Suggested viewport matrix

| Profile | Approximate viewport | Review |
|---|---:|---|
| Small mobile | 320 × 640 | Horizontal overflow, image clipping, target size |
| Typical mobile | 390 × 844 | Card width, carousel height, navigation wrapping |
| Tablet | 768 × 1024 | Spacing, alignment, dropdown position |
| Desktop | 1366 × 768 | Content balance and image scaling |
| Wide desktop | 1920 × 1080 | Maximum content width and excess whitespace |

These are suggested test sizes, not certified support claims.

## 3. Task 1 card

Check that the card fits narrow viewports. Prefer a responsive container and viewport-aware maximum width rather than a fixed width that can exceed the available screen.

## 4. Task 2 carousel

Confirm images scale with the carousel container, controls remain visible, and the slide height does not create unwanted layout shifts.

## 5. Task 3 navigation

The Login button uses a large inline left margin. This may push content off-screen on smaller viewports. Prefer Bootstrap flex alignment and responsive spacing utilities. Confirm dropdown placement and modal sizing at mobile widths.

## 6. Reflow and zoom

Test 200% zoom and larger text settings. Avoid fixed heights that clip content. Ordinary content should not require two-dimensional scrolling at narrow widths.

## 7. Review evidence

For UI changes, record the browser, viewport, expected behavior, actual result, and genuine screenshots in the pull request.
