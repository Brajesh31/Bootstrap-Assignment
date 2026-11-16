# 🖼️ Runbook: Asset Verification

## Purpose

Verify that each task page can load its local image assets and that image reuse rights are understood before public redistribution.

## Path verification

1. Open the task HTML page.
2. Inspect each image `src` value.
3. Resolve the path relative to the HTML file's URL.
4. Confirm the exact file exists in `Assignment_14_Bootstrap/media/`.
5. Check filename casing.
6. Inspect the Network panel for 404s.
7. Confirm images scale without distortion.

## Rights verification

For each media asset, locate the original source and record the owner, license, attribution requirement, and redistribution permission. Do not infer that the root MIT license covers third-party images.

## Accessibility verification

- Replace placeholder alt text with a concise description of meaningful content.
- Use an empty alt value for purely decorative images.
- Avoid placing important information only inside an image.

## Completion criteria

All page image references resolve, image descriptions are accurate, and known licensing gaps are recorded. Do not claim an image is cleared for redistribution without evidence.
