# Architecture

## Overview

Bootstrap Assignment is a static website exercise. Each HTML document is a separate page; the browser parses the page, loads its local images, and fetches Bootstrap CSS and JavaScript from jsDelivr. There is no build pipeline, app framework, application server, persistent data store, or API.

~~~text
Browser
  ├── Task_1.html: course card
  ├── Task_2.html: image carousel
  └── Task_3.html: navigation, dropdown, login modal
       ├── media/: local image assets
       └── jsDelivr: Bootstrap 5.3.2 CSS and JavaScript bundle
~~~

## Pages and components

- Task_1.html contains a Bootstrap card with a local course image, title, descriptive text, and an Enroll Now anchor. The anchor currently points to # and does not enroll a user.
- Task_2.html contains a dark carousel with three local images, three indicators, timed slides, and previous/next controls. Bootstrap's JavaScript bundle provides the interaction.
- Task_3.html contains a tab-style navigation list, a local logo, a Courses dropdown, two placeholder navigation links, and a button that opens a Bootstrap modal. The modal form shows email and password fields but has no submission handler or authentication service.

All image paths are relative to the HTML files and point into media/. The output/ directory contains saved rendered examples; the pages do not load those output files.

## Dependencies and runtime

Bootstrap CSS and the Bootstrap JavaScript bundle are versioned at 5.3.2 and loaded from jsDelivr with subresource integrity and crossorigin metadata. No local Bootstrap copy is included. Interactive dropdown, carousel, and modal features depend on loading the JavaScript bundle. Styling and those interactions can fail if the CDN is unavailable.

The HTML can be opened directly with a browser or served by any static file server. The static server's document root should be the Assignment_14_Bootstrap directory if the task pages are to be served at its root. The repository root itself has no index page.

## Boundaries

There are no network calls from project-authored application code, no form submission, and no account or enrollment backend. The remote CDN requests are the only required runtime network dependency described by the markup. Media ownership and reuse permissions are not recorded in the source; check them before redistribution.
