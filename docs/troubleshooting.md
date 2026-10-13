# Troubleshooting

## The page has no Bootstrap styling

Check your internet connection and browser developer console. The stylesheets are loaded from jsDelivr; this repository does not include a local copy of Bootstrap. A blocked CDN request will leave the page with browser-default styling.

## The carousel, dropdown, or modal does not respond

These controls require the Bootstrap 5.3.2 JavaScript bundle. Confirm that the bundle request succeeds and that the page's Bootstrap CSS and JavaScript versions and integrity values match the intended upstream files. Check the browser console for failed network or integrity errors.

## Images are missing

Open the HTML from its existing location or serve the Assignment_14_Bootstrap directory as the web root. The page expects image files under the sibling media/ directory. Preserve both the file names and folder relationship when copying or deploying the pages.

## The repository root displays a directory listing or blank page

There is no index.html at the repository root. Open a task page directly or configure a static host to publish Assignment_14_Bootstrap as the document root.

## The login form does nothing

That is the current design: the modal is a Bootstrap UI exercise only. There is no action URL, JavaScript submit handler, or authentication service. Do not enter actual credentials.

## Enroll Now or navigation links do not go anywhere

The anchors currently use # as placeholder destinations. They need real destinations before being used as navigation or enrollment actions.

## The page looks cramped on a phone

Review the viewport layout and Bootstrap grid/spacing classes at narrow widths. Task_3 uses a large inline margin on the Login button, which may not adapt well to smaller screens.

## Local file preview behaves differently

Start a basic static server in Assignment_14_Bootstrap with python -m http.server 8000 and visit a page through localhost. This project does not require a server for its current HTML and image paths, but serving files over HTTP can make browser inspection more consistent.
