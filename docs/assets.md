# 🖼️ Media and Screenshot Inventory

## 1. Purpose

This document explains the existing visual assets and how they are used. It does not claim ownership or license rights for images whose provenance is not recorded.

## 2. Existing media assets

| File | Format | Referenced by |
|---|---|---|
| `media/64a514966977cc6e87e27504.png` | PNG | Task 1 course card |
| `media/653b999fd85a4d9660adf574.png` | PNG | Task 2 carousel slide |
| `media/6568179250c244fbec73aaf4.jpg` | JPEG | Task 2 carousel slide |
| `media/6569744750c244a030749278.jpg` | JPEG | Task 2 carousel slide |
| `media/1681225007-6197.png` | PNG | Task 3 navigation logo |

## 3. Saved output renders

| File | Purpose |
|---|---|
| `output/task_1.png` | Saved example render for Task 1 |
| `output/task_2.png` | Saved example render for Task 2 |
| `output/task_3_a.png` | Saved example render for Task 3 |
| `output/task_3_b.png` | Additional saved example render for Task 3 |

These are reference renders. The HTML pages do not load files from the output directory.

## 4. Image path convention

The HTML files and `media/` folder are siblings. Image sources use relative paths such as:

```html
<img src="media/example.png" alt="Accurate image description">
```

If a task page is moved, its relative image paths must be updated or the folder layout preserved.

## 5. Provenance and licensing workflow

Before adding or redistributing an image, record:
- Filename and purpose.
- Original source URL or creator.
- Copyright owner.
- License or written permission.
- Required attribution.
- Date and person who verified permission.

The root MIT license covers the repository code according to its terms. It does not automatically provide permission to redistribute every image in media/.

## 6. Quality requirements

- Use descriptive alt text for meaningful images.
- Use empty alt text for purely decorative images.
- Optimize images to reasonable rendered dimensions.
- Preserve aspect ratio.
- Avoid embedding credentials, personal data, or private screenshots.
- Keep genuine application screenshots separate from illustrative mockups.
