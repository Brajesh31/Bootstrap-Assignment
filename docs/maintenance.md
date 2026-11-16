# 🔧 Maintenance Guide

## Routine maintenance checklist

### HTML
- Recheck titles, headings and semantic landmarks.
- Verify all internal IDs and links.
- Ensure labels and alt text are accurate.
- Remove placeholder destinations before promoting the pages for real use.

### Bootstrap
- Review Bootstrap release notes before upgrades.
- Keep CSS and JS versions aligned.
- Recheck SRI hashes against the exact files.
- Test carousel, dropdown and modal after each update.

### Media
- Check broken image requests.
- Review image file sizes and dimensions.
- Confirm ownership and reuse rights.
- Keep the output screenshots distinct from runtime media.

### Documentation
- Update the documentation hub when adding or renaming guides.
- Update diagrams when component IDs or behavior changes.
- Keep limitations accurate.
- Do not describe visual examples as production capabilities.

## Periodic review

At a practical interval, review external CDN dependencies, browser compatibility, accessibility, mobile layout, image rights, root README links, and GitHub Actions status.

## Change hygiene

Keep changes focused. Avoid adding a framework, backend, database, or test suite unless it is justified by a real scope change.
