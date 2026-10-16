# Bootstrap Assignment

A small collection of static HTML exercises built with Bootstrap 5.3.2. The project demonstrates a course card, an image carousel, and a navigation layout with a dropdown and login modal. It is an educational front-end sample, not a complete course platform or authentication application.

## Exercises

| Page | Demonstration |
| --- | --- |
| Assignment_14_Bootstrap/Task_1.html | A centered course card with an image, course description, and Enroll Now link. |
| Assignment_14_Bootstrap/Task_2.html | A dark Bootstrap carousel with three local images, indicators, timed slides, and previous/next controls. |
| Assignment_14_Bootstrap/Task_3.html | A Bootstrap tab-style navigation bar with a local logo, Courses dropdown, placeholder navigation links, and a login modal form. |

The existing rendered examples are stored in Assignment_14_Bootstrap/output/. Images used by the pages are in Assignment_14_Bootstrap/media/. Keep the relative media paths intact when moving or publishing the HTML files.

## Preview locally

No build step, package manager, or server-side runtime is required. Open any Task HTML file directly in a modern browser. For a local HTTP preview, run a static server from the exercise directory:

~~~powershell
cd Assignment_14_Bootstrap
py -m http.server 8000
~~~

Then open http://localhost:8000/Task_1.html, /Task_2.html, or /Task_3.html. If the py launcher is unavailable, use python -m http.server 8000.

The pages load Bootstrap CSS and the Bootstrap JavaScript bundle from jsDelivr. An internet connection is needed for those CDN assets. Without them, the pages' own HTML and local images remain available, but Bootstrap styling and interactive components may not work as intended.

## Repository layout

~~~text
Assignment_14_Bootstrap/
├── Task_1.html
├── Task_2.html
├── Task_3.html
├── media/       # Images referenced by the pages
└── output/      # Saved example renders
docs/            # Project and contributor documentation
~~~

## Current scope and limitations

This repository contains only static HTML and image assets. It has no JavaScript application code, API, database, environment configuration, user accounts, or real login/enrollment flow. The navigation links and Enroll Now link currently point to #. The login modal displays email and password fields, but it does not submit or authenticate credentials. Do not enter real credentials into this demo.

Some image alt attributes are placeholders and should be replaced with meaningful descriptions if the pages are adapted for broader use. Image provenance and reuse permissions are not documented by the source files; verify them before redistributing the images. The MIT license applies to the project code and does not grant rights to third-party assets.

## Contributing and support

See CONTRIBUTING.md for making changes, CODE_OF_CONDUCT.md for community expectations, SECURITY.md for private security reporting, and SUPPORT.md for help. The docs directory includes installation, architecture, development, deployment, route, data, troubleshooting, and FAQ information.

## License

The project code is available under the MIT License. See LICENSE.

Last updated: 2026-10-16 02:13 UTC
