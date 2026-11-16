# 🌐 Browser Compatibility and Verification Guide

## 1. Purpose

This guide defines a practical compatibility target for the three static Bootstrap pages. It is a verification plan, not a claim that every browser/version has already been tested.

The pages rely on semantic HTML, Bootstrap 5.3.2 CSS and JavaScript delivered by jsDelivr, and local image files. Browser behavior therefore depends on both the browser and the availability of the external CDN.

## 2. Compatibility target

Use current stable releases of the following browser families when performing a manual review:

| Browser family | Desktop check | Mobile check | Notes |
|---|---|---|---|
| Google Chrome / Chromium | Required | Android Chrome where available | Check layout, carousel, dropdown and modal |
| Mozilla Firefox | Required | Firefox Android where available | Check focus behavior and responsive sizing |
| Microsoft Edge | Required | Not a primary target | Chromium-based desktop verification |
| Apple Safari | Required where available | iOS Safari | Pay attention to viewport sizing and native form controls |

Do not publish a specific browser version as supported unless it has actually been tested. Record the exact browser version, operating system, viewport size, date, and result in the QA record.

## 3. Page-level checks

### Task 1: Course card
- Confirm the card remains readable at narrow, medium, and wide viewport widths.
- Confirm the image loads from the relative media path.
- Confirm the card does not create horizontal page overflow.
- Check text wrapping and link focus visibility.
- Confirm the Enroll Now placeholder is clearly understood as non-functional.

### Task 2: Carousel
- Confirm all three local slides load.
- Use previous and next controls with mouse, touch, and keyboard where supported.
- Confirm indicators select the expected slide.
- Observe automatic cycling and verify it does not make content impossible to read.
- Check image cropping and container height at portrait and landscape widths.
- Verify that disabling JavaScript leaves the limitation understandable rather than implying a working interactive carousel.

### Task 3: Navigation and modal
- Open and close the Courses dropdown using pointer and keyboard.
- Open the login modal and close it with its close control and Escape.
- Move through fields using Tab and Shift+Tab.
- Confirm focus is visible and does not become trapped outside the modal.
- Resize the viewport while the modal is open and check scrolling.
- Do not enter real credentials. The form is a visual demonstration and has no authentication handler.

## 4. Responsive viewport matrix

Use these representative viewport widths as test points, not as a statement of device certification:

| Class | Example width | Main concerns |
|---|---:|---|
| Small phone | 320 px | Overflow, cramped controls, text wrapping |
| Typical phone | 375-390 px | Card width, carousel crop, modal fit |
| Large phone | 430 px | Spacing and image scaling |
| Tablet portrait | 768 px | Navigation and content alignment |
| Laptop | 1366 px | Main content width and whitespace |
| Desktop | 1920 px | Excessive stretching and image quality |

## 5. CDN and offline behavior

The Bootstrap stylesheet and JavaScript are external dependencies. Test both:
1. **Online:** confirm the CDN requests succeed and interactive components initialize.
2. **Offline or blocked CDN:** confirm local HTML and images still load, while documenting that Bootstrap styling and JavaScript-driven behavior may be unavailable.

Do not silently replace CDN dependencies or remove Subresource Integrity attributes during compatibility fixes.

## 6. Reporting a compatibility defect

Include the page path, browser name and exact version, operating system and device type, viewport dimensions and zoom level, reproduction steps, expected and actual behavior, screenshot or short recording where safe, and whether the issue reproduces in a fresh browser session.

## 7. Evidence and status

No browser certification is implied by this document. Record only tests that were actually performed. A useful status is **Not tested**, **Pass**, **Fail**, or **Blocked**, with a date and evidence reference.

Related guides: [Testing](testing.md), [Responsive Design](responsive-design.md), [Accessibility](accessibility.md), and [Troubleshooting](troubleshooting.md).
