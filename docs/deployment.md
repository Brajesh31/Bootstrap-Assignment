# 🌐 Deployment Guide

## 1. Hosting model

This repository is a static collection of HTML pages and image assets. It does not require a backend process, build output, database, package installation, or environment variables.

The repository root does not contain an `index.html`. The three task pages are under `Assignment_14_Bootstrap/`.

## 2. Choose the document root

**Option A: publish the assignment directory as the site root.** The host document root points to the contents of `Assignment_14_Bootstrap/`. Visitors can open `/Task_1.html`, `/Task_2.html`, and `/Task_3.html`.

**Option B: publish the repository root.** The pages remain nested at `/Assignment_14_Bootstrap/Task_1.html`, etc. Configure navigation or a landing page separately if a friendly root URL is needed.

Do not assume that the host automatically selects one of the task pages.

## 3. Files to publish

Include all three HTML files and the complete `media/` directory. The `output/` directory contains saved example renders and is useful as reference material, but the pages do not load those images.

Preserve directory layout and filename casing because the HTML uses relative media paths.

## 4. External dependency requirements

Bootstrap 5.3.2 CSS and JavaScript are loaded from jsDelivr. Users need network access to the CDN for full styling and interactive carousel/dropdown/modal functionality.

Verify the version and SRI hashes before deployment. A local Bootstrap distribution is an optional future change, not currently included.

## 5. Production caveat

The login modal and enrollment link are examples only. Do not publish them as working authentication or course enrollment services. A real user system requires a backend, privacy review, security controls, and operational ownership.

## 6. Post-deployment checks

- [ ] All task URLs return the expected HTML.
- [ ] All local images load.
- [ ] Bootstrap CDN requests succeed.
- [ ] Carousel controls work.
- [ ] Dropdown opens and closes.
- [ ] Modal opens and closes.
- [ ] Mobile layout remains usable.
- [ ] No real credential collection is implied.
- [ ] Image distribution rights are verified.

## 7. Rollback

Because the site is static, restore the previous known-good deployment artifact or publish the previous reviewed commit. Verify all HTML and media paths after rollback.
