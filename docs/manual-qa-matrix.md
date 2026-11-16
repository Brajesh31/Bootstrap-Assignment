# 🧪 Manual Quality Assurance Matrix

## 1. Purpose and test policy

This matrix is the repeatable manual test record for the three HTML exercises. It describes checks to perform. A listed test is not evidence that the test has passed.

The project currently has lightweight automated repository checks, but it does not have a browser-driven end-to-end suite. Record actual results and do not convert planned checks into fabricated pass statuses.

## 2. Test environment record

For each test session, record:
- Date and time of test.
- Tester.
- Git commit SHA under test.
- Operating system and version.
- Browser name and exact version.
- Viewport dimensions in CSS pixels.
- Network condition: online, throttled, or offline.
- Result: Pass, Fail, Blocked, or Not tested.
- Evidence: screenshot, issue URL, or notes.

## 3. Functional test cases

| ID | Page | Action | Expected result | Result |
|---|---|---|---|---|
| QA-001 | Task 1 | Open page | Page loads without a missing local image | Not tested |
| QA-002 | Task 1 | Resize viewport | Card remains readable without horizontal overflow | Not tested |
| QA-003 | Task 1 | Activate Enroll Now | Placeholder behavior is understood; no real enrollment is claimed | Not tested |
| QA-004 | Task 2 | Open page | Carousel and first local image render | Not tested |
| QA-005 | Task 2 | Select each indicator | Corresponding slide becomes active | Not tested |
| QA-006 | Task 2 | Use previous/next controls | Carousel moves one slide in the expected direction | Not tested |
| QA-007 | Task 2 | Wait through an interval | Automatic slide behavior matches the page configuration | Not tested |
| QA-008 | Task 3 | Open Courses dropdown | Menu opens and its items are readable | Not tested |
| QA-009 | Task 3 | Open login modal | Modal appears and the page backdrop behaves correctly | Not tested |
| QA-010 | Task 3 | Close modal with close control | Modal closes and focus returns sensibly | Not tested |
| QA-011 | Task 3 | Press Escape while modal is open | Modal closes when Bootstrap's configured behavior permits | Not tested |
| QA-012 | Task 3 | Tab through controls | Focus remains visible and follows a logical order | Not tested |

## 4. Cross-cutting quality checks

| ID | Area | Check | Expected result | Result |
|---|---|---|---|---|
| QA-013 | Assets | Inspect all relative image paths | Every referenced local image exists | Not tested |
| QA-014 | Accessibility | Inspect image alternatives | Informative images have meaningful alt text; decorative images are handled appropriately | Not tested |
| QA-015 | Accessibility | Keyboard-only review | Interactive controls can be reached and operated | Not tested |
| QA-016 | Responsive | Test the viewport matrix | No unintended horizontal overflow or clipped controls | Not tested |
| QA-017 | CDN | Load with network access | Bootstrap resources load successfully | Not tested |
| QA-018 | Offline | Block external CDN requests | Local HTML and media remain available; CDN-dependent behavior is documented | Not tested |
| QA-019 | Security | Inspect Task 3 form | No real credential submission or storage occurs | Not tested |
| QA-020 | Documentation | Follow local Markdown links | Internal documentation links resolve | Not tested |

## 5. Defect severity

- **Critical:** exposed secrets, unexpected credential handling, or a defect that makes the repository unsafe to use.
- **High:** a core exercise cannot load or a primary control is unusable.
- **Medium:** a significant layout, browser, or accessibility defect with a practical workaround.
- **Low:** cosmetic issue, typo, or minor inconsistency.

Severity should reflect actual impact, not the amount of code changed.

## 6. Regression procedure

After editing a task page:
1. Review the source diff and confirm unrelated files were not changed.
2. Run the repository's GitHub Actions checks.
3. Open the changed page locally.
4. Repeat its page-specific test cases.
5. Repeat relevant cross-cutting checks for images, keyboard use, responsive layout, and CDN behavior.
6. Update this matrix only with the result of a test actually performed.
7. Link any failure to an issue with reproduction steps and evidence.

## 7. Related resources

- [Testing guide](testing.md)
- [Browser compatibility](browser-compatibility.md)
- [Accessibility](accessibility.md)
- [Responsive design](responsive-design.md)
- [Troubleshooting](troubleshooting.md)
