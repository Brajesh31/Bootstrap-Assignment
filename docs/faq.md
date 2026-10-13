# Frequently asked questions

## What is this repository?

It is a small set of Bootstrap 5.3.2 HTML exercises: a course card, an image carousel, and a navigation bar with a dropdown and modal.

## How do I start it?

Open one of the three Task HTML pages in a browser. For a local HTTP preview, serve the Assignment_14_Bootstrap directory using Python's built-in static server. See installation.md for commands.

## Do I need Node.js or a build step?

No. The project has no package manifest or build pipeline. Bootstrap is loaded from jsDelivr at runtime.

## Why does the project need internet access?

The HTML references Bootstrap CSS and the JavaScript bundle from jsDelivr. The pages also use local images. The interactive carousel, dropdown, and modal need the Bootstrap bundle to load.

## Does the login modal authenticate users?

No. It only displays sample input fields and buttons. It has no server, submission handler, or credential storage. Never enter real passwords.

## Does Enroll Now register me for a course?

No. The link is a placeholder with a # destination.

## Is there an API or database?

No. All content is static HTML and image files; there are no API endpoints, database, or persistent user records.

## Can the images be reused under the MIT license?

The MIT license covers the source code as stated in LICENSE. It does not establish image ownership or usage rights. Verify the rights and source of each image before reuse.

## Where can I ask questions or report issues?

Use the repository's GitHub Issues page for ordinary questions and reproducible defects. For suspected security issues, follow SECURITY.md and report privately.
