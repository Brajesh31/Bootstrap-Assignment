# ❓ Frequently Asked Questions

## What does this repository contain?

Three standalone Bootstrap HTML exercises: a course card, an image carousel, and a navigation bar with dropdown and login modal.

## Which Bootstrap version is used?

The pages reference Bootstrap 5.3.2 CSS and JavaScript from jsDelivr.

## Do I need Node.js or npm?

No. There is no package manifest or build step. A browser is enough to open the HTML files. Python can optionally serve them over HTTP.

## Why do some components fail without internet?

Bootstrap CSS and JavaScript are loaded from jsDelivr. Without the CDN, styling and JavaScript-powered carousel, dropdown, and modal behavior may not work.

## Does Login authenticate a user?

No. It opens a presentation-only modal with email and password fields. It has no submit handler, API, or credential storage. Never enter real credentials.

## Does Enroll Now enroll a student?

No. The anchor points to `#` and does not connect to an enrollment service.

## Is there a database?

No. The project is static HTML and local image files.

## What is the output directory?

It contains saved rendered examples. The HTML pages do not load those files at runtime.

## Can I reuse the images under the MIT license?

The repository's MIT license does not automatically grant rights to third-party images. Verify the source and usage license of each image before redistribution.

## How do I report a bug?

Open a GitHub issue with the task page, browser, viewport, exact steps, expected behavior, observed behavior, and sanitized console output.

## How do I report a vulnerability?

Use the private process described in the root SECURITY.md. Do not publish secrets or exploit details in a public issue.
