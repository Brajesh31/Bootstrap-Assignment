# 🧪 Testing and Verification Guide

## 1. Current test baseline

There is no automated test suite, package.json, test runner, browser automation, or custom application JavaScript in the current repository. The appropriate baseline is a repeatable manual browser test matrix.

## 2. Preview setup

Open the HTML directly, or serve the assignment folder:

```bash
cd Assignment_14_Bootstrap
python3 -m http.server 8000
```

Open each page from `http://localhost:8000/`.

## 3. Task-level test matrix

| ID | Page | Action | Expected result |
|---|---|---|---|
| T1-01 | Task 1 | Load page | Course card is visible |
| T1-02 | Task 1 | Inspect image | Local course image loads |
| T1-03 | Task 1 | Activate Enroll Now | Current placeholder remains on page; no enrollment service |
| T2-01 | Task 2 | Load page | Carousel shows first active slide |
| T2-02 | Task 2 | Activate each indicator | Matching slide appears |
| T2-03 | Task 2 | Use Previous/Next | Carousel changes slides |
| T2-04 | Task 2 | Wait for interval | Automatic slide transition occurs when Bootstrap JS loads |
| T3-01 | Task 3 | Open Courses dropdown | Menu opens |
| T3-02 | Task 3 | Dismiss dropdown | Menu closes appropriately |
| T3-03 | Task 3 | Click Login | Modal opens |
| T3-04 | Task 3 | Click close/Close | Modal closes |
| T3-05 | Task 3 | Inspect fields | Labels match email and password inputs |
| T3-06 | Task 3 | Click Login footer control | No authentication should be assumed |

## 4. Cross-page checks

- Verify all local image requests return successfully.
- Verify Bootstrap CSS and JS CDN requests succeed.
- Inspect browser console for SRI or JavaScript errors.
- Test at a narrow mobile viewport and desktop width.
- Navigate using keyboard only.
- Verify focus is visible.
- Test browser zoom and text enlargement.
- Check alt text and heading order.

## 5. Accessibility checks

Automated scanning can supplement but not replace:
- Keyboard testing.
- Screen-reader spot checks.
- Contrast evaluation.
- Motion/auto-rotation review.
- Form-label verification.

## 6. Regression evidence

Record browser, viewport, page, steps, expected and actual results, and any console/network errors. Use genuine screenshots from the actual rendered pages. The existing `output/` files are saved example renders; do not treat them as evidence of a newly tested build without rerunning the tests.

## 7. Future automation

If this repository evolves, a lightweight HTML validator and Playwright smoke tests could be introduced. Add them only with a documented installation path and meaningful assertions.
