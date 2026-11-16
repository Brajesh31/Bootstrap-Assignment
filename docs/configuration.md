# ⚙️ Configuration and Dependency Guide

## 1. Current configuration model

The pages are plain HTML. There is no JavaScript build configuration, package.json, bundler, server runtime configuration, or application environment loader.

The meaningful configuration is located in the HTML markup itself:
- Bootstrap version and CDN URL.
- Subresource Integrity (SRI) hashes and crossorigin attributes.
- Carousel slide intervals and target IDs.
- Relative local media paths.
- Bootstrap data attributes for carousel, dropdown and modal behavior.

## 2. Bootstrap version consistency

The current pages reference Bootstrap 5.3.2 CSS and JavaScript from jsDelivr. Keep both assets on the same version. When upgrading:
1. Select the target Bootstrap release.
2. Update every page consistently.
3. Obtain integrity hashes for the exact downloaded files.
4. Keep `crossorigin="anonymous"` where applicable.
5. Test carousel, dropdown, modal and responsive behavior.
6. Review release notes for breaking changes.

Do not copy an integrity value from a different Bootstrap release or a different minified file.

## 3. CDN and offline behavior

Bootstrap is not vendored locally. A network connection is needed to retrieve the CSS and JavaScript bundle. Without the CDN:
- Browser-native HTML remains available.
- Local images can still load.
- Bootstrap layout and component styling will be missing.
- Carousel, dropdown and modal behavior may not work.

A local vendored copy is an optional future improvement. It must be versioned, licensed, updated for security fixes, and documented.

## 4. Carousel settings

Task 2 sets per-slide `data-bs-interval` values. Values are milliseconds. If changing timing:
- Keep the interval long enough to read meaningful content.
- Consider visitors who need more time.
- Provide a way to pause or stop automatic rotation when appropriate.
- Test indicators and previous/next controls.
- Check reduced-motion expectations.

## 5. Environment variables

No page reads environment variables. The `.env.example` does not configure a working runtime. Never place credentials in static HTML or client-side code.

## 6. Configuration audit checklist

- [ ] Bootstrap CSS and JS versions match.
- [ ] SRI hashes match the exact remote assets.
- [ ] Every local media path resolves.
- [ ] Carousel indicators match slide count.
- [ ] Dropdown and modal targets match element IDs.
- [ ] No secrets or real credentials appear in source.
