# Development

## Source layout

- Assignment_14_Bootstrap/Task_1.html: card exercise.
- Assignment_14_Bootstrap/Task_2.html: carousel exercise.
- Assignment_14_Bootstrap/Task_3.html: navigation, dropdown, and modal exercise.
- Assignment_14_Bootstrap/media/: local images used by the pages.
- Assignment_14_Bootstrap/output/: saved rendered examples.
- docs/: project documentation.

There is no build configuration, custom JavaScript, custom stylesheet, package manifest, lint configuration, automated test suite, or CI workflow in the project.

## Editing workflow

Edit the HTML page that owns the behavior or layout. Keep page assets in media/ and preserve relative paths. Use Bootstrap classes already available through the CDN rather than adding a separate framework without documenting it.

When updating Bootstrap, use a consistent CSS and JavaScript version and verify the subresource integrity values against the exact files being requested. The carousel, dropdown, and modal depend on the bundled JavaScript. The card's link and the navigation links are placeholders, and the login form has no submit behavior; do not imply these features are connected to a real service.

Prefer meaningful page titles, semantic landmarks, visible focus states, labels connected to controls, and accurate alt text. Review the layout at narrow and wide viewport sizes. Add only images that may legally be redistributed and document their source.

## Manual review

No automated tests are provided. For a change to a page, open that page in a browser and review its layout, local images, keyboard behavior, and relevant Bootstrap interaction. For Task_2, check all indicators and previous/next controls. For Task_3, open and close the dropdown and modal, and confirm the form does not expose or transmit real credentials. Mention the review performed in the pull request.

## Data and privacy

The pages contain no application data store or user accounts. The modal's email/password controls are visual sample fields only. Do not enter or request real credentials.
