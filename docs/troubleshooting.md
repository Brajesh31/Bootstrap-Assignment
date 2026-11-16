# 🧯 Troubleshooting

## 1. Bootstrap styles are missing

The pages load Bootstrap CSS from jsDelivr. Check internet access, browser console, and Network panel. The repository does not include a local Bootstrap distribution.

## 2. Carousel does not move

- Confirm the Bootstrap JavaScript bundle request succeeds.
- Check for SRI errors in the console.
- Confirm the carousel root ID matches every indicator/control target.
- Confirm there is one active carousel item.
- Confirm indicator slide indexes match the actual item order.

## 3. Dropdown does not open

Check that Bootstrap's JavaScript bundle is loaded and the dropdown trigger uses `data-bs-toggle="dropdown"`. Check that dropdown menu markup is nested correctly.

## 4. Login modal does not open

Confirm the Login button's `data-bs-target` matches the modal's `id`. Confirm Bootstrap JavaScript loaded successfully. The modal is a UI demonstration and does not authenticate users.

## 5. Images do not load

Serve the `Assignment_14_Bootstrap/` directory as the document root, or open the HTML from its existing folder. The HTML expects a sibling `media/` directory. Preserve capitalization and exact file names.

## 6. Root page is missing

There is no root `index.html`. Open one of the Task pages directly or configure the static host to publish the assignment directory as the document root.

## 7. Enroll Now or nav links do nothing

Several anchors use `href="#"` as placeholders. They need real page destinations before they can function as navigation or enrollment actions.

## 8. Mobile layout is cramped

Inspect Task 3's large inline margin on the Login button and the nav list's flex classes. Use responsive Bootstrap utilities and test at narrow widths. Avoid fixed offsets that force content off-screen.

## 9. Output screenshots are not shown in the page

The `output/` directory contains reference images, not page assets. The HTML pages reference files under `media/`.

## 10. File:// behavior differs from server preview

Run a static server from `Assignment_14_Bootstrap/` using `python -m http.server 8000` and open a localhost URL.
