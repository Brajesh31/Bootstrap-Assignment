# 🧭 Usage Guide

## 1. Opening the exercises

Open one HTML file under `Assignment_14_Bootstrap/` in a browser, or serve that directory over HTTP using Python. The exercise pages are independent.

## 2. Task 1: course card

1. Open `Task_1.html`.
2. Review the course image, heading and description.
3. Inspect the Enroll Now link.

The link is a placeholder with `href="#"`. It does not register a learner. Do not interpret it as a working enrollment process.

## 3. Task 2: image carousel

1. Open `Task_2.html`.
2. Use the indicators to jump to a slide.
3. Use Previous and Next controls to move between images.
4. Observe automatic timing configured by each slide's `data-bs-interval`.

The carousel requires the Bootstrap JavaScript bundle to load. The slides use local images. If you modify the slide count, update indicators and controls consistently.

## 4. Task 3: navigation and login modal

1. Open `Task_3.html`.
2. Activate Courses to open the dropdown.
3. Inspect the placeholder menu items and navigation links.
4. Activate Login to open the modal.
5. Review the email/password fields.
6. Close the modal using the close icon or Close button.

The Login button is not connected to an authentication flow. The form has no submission handler. Never enter real credentials.

## 5. Browser developer tools

Use the browser's developer tools to:
- Inspect HTML and Bootstrap classes.
- Check CDN requests in the Network panel.
- Review console errors.
- Verify image requests and natural dimensions.
- Test keyboard focus and modal dismissal.
- Inspect responsive layout at mobile and desktop widths.

## 6. Modifying the examples

Keep assets in the `media/` directory and preserve relative paths. For Task 2, maintain the relationship between indicators and carousel items. For Task 3, keep `data-bs-target` values synchronized with modal and dropdown IDs. Update the docs if behavior or Bootstrap versions change.
