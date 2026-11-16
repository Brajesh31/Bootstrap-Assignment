# 🚀 Runbook: Static Publishing

## Purpose

Prepare a static copy of the assignment for a host that serves HTML and image files.

## Pre-publish checklist

- [ ] Confirm the three task pages are included.
- [ ] Include the complete media directory.
- [ ] Preserve relative path structure and filename case.
- [ ] Decide whether the document root is the repository root or the assignment directory.
- [ ] Confirm Bootstrap CDN requests and SRI hashes.
- [ ] Inspect all placeholder links and avoid presenting them as real services.
- [ ] Confirm login modal is clearly a UI demonstration.
- [ ] Verify image reuse rights.
- [ ] Test the pages at mobile and desktop widths.
- [ ] Check keyboard behavior, focus and alt text.

## Publish

Publish the static files using the configured hosting provider. There is no provider-specific deployment command in this repository. Do not assume a root index page exists.

## Post-publish verification

Open each deployed task URL. Confirm HTML, local media and Bootstrap CDN assets load. Exercise the carousel, dropdown and modal. Check browser console and network errors.

## Rollback

Restore the previous verified static artifact or publish the previous reviewed commit. Check media path behavior after rollback.
