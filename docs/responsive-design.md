# 📱 Responsive Design Guide

## 1. Purpose

The three exercises use Bootstrap 5.3.2 classes, but their layouts still need to be verified at different viewport sizes. The presence of Bootstrap does not guarantee that every custom inline style or content choice is responsive.

## 2. Suggested viewport matrix

| Profile | Approximate viewport | What to review |
|---|---:|---|
| Small mobile | 320 × 640 | Horizontal overflow, image clipping, control size |
| Typical mobile | 390 × 844 | Card width, carousel height, nav wrapping |
| Tablet | 768 × 1024 | Spacing, navigation alignment, modal dimensions |
| Desktop | 1366 × 768 | Content balance and image scaling |
| Wide desktop | 1920 × 1080 | Maximum content width and excessive whitespace |

These are suggested test viewports, not measured support claims.

## 3. Task 1 card

Check that the card does not overflow narrow screens. Prefer a responsive container and a width constrained by the viewport instead of a fixed card width that can exceed a small device.

## 4. Task 2 carousel

Check that each image scales with the carousel container and that controls remain visible. Ensure image dimensions do not cause unexpected page shifts.

## 5. Task 3 navigation

The Login button currently uses a large inline left margin. This can push content out of the viewport at smaller widths. Prefer Bootstrap flex alignment and responsive spacing utilities. Confirm dropdown placement and modal dimensions at mobile widths.

## 6. Reflow and zoom

Test 200% zoom and larger text settings. The page should remain usable without horizontal scrolling for ordinary content. Avoid fixed heights that clip text.

## 7. Review record

For UI changes, include actual browser, viewport, expected behavior, observed behavior, and screenshots in the pull request.
