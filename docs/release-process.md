# 🚢 Release Process

## Release model

A release is a reviewed snapshot of static HTML pages and their local media. There is no build pipeline or application runtime to deploy.

## Pre-release checklist

- [ ] Review changes to all Task HTML files.
- [ ] Confirm relative media paths.
- [ ] Verify Bootstrap version and SRI hashes.
- [ ] Open Task 1 and verify its card layout.
- [ ] Open Task 2 and test indicators and previous/next controls.
- [ ] Open Task 3 and test dropdown and modal behavior.
- [ ] Test keyboard access and narrow viewport behavior.
- [ ] Review image rights and alt text.
- [ ] Confirm login and enrollment placeholders are not presented as live services.
- [ ] Update README and docs if the project behavior changed.

## Release notes

Summarize task-specific changes, media updates, framework upgrades, known limitations, and manual test coverage. Do not claim a release or public deployment unless it actually occurred.

## Rollback

Restore the last known-good static artifact or publish the previous reviewed commit. Confirm image paths and CDN dependencies after rollback.
