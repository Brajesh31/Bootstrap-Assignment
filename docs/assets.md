# 🖼️ Media and Screenshot Inventory

## 1. Purpose

This document explains the existing visual assets and their use. It does not claim ownership or license rights for images whose provenance is not recorded.

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
| `output/task_1.png` | Saved Task 1 example render |
| `output/task_2.png` | Saved Task 2 example render |
| `output/task_3_a.png` | Saved Task 3 example render |
| `output/task_3_b.png` | Additional Task 3 example render |

These are reference renders. The task HTML files do not load images from the output directory.

## 4. Relative path convention

The task HTML files and `media/` directory are siblings. Image sources use relative paths such as:

```html
<img src="media/example.png" alt="Accurate image description">
```

If a task page is moved, its relative image paths must be updated or the folder structure preserved.

## 5. Provenance and licensing

Before adding or redistributing an image, record its filename, purpose, original source/creator, copyright owner, license or permission, attribution requirements, and verification date. The root MIT license applies to project code according to its terms; it does not automatically permit redistribution of every image in `media/`.

## 6. Quality requirements

Use meaningful alt text for informative images, empty alt text for decorative images, optimize file sizes, preserve aspect ratio, and avoid private data in screenshots.
