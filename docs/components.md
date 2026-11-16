# 🧱 Bootstrap Component Reference

## 1. Component inventory

| Task | Component | Selector/class | Bootstrap JavaScript required? |
|---|---|---|---|
| 1 | Card | `.card`, `.card-img-top`, `.card-body` | No |
| 2 | Carousel | `.carousel`, `.carousel-inner`, `.carousel-item` | Yes |
| 3 | Navigation tabs | `.nav`, `.nav-tabs`, `.nav-link` | No for basic visual nav layout |
| 3 | Dropdown | `.dropdown`, `.dropdown-menu` | Yes |
| 3 | Modal | `.modal`, `.modal-dialog`, `.modal-content` | Yes |
| 3 | Form controls | `.form-control`, `.form-label` | No for native input behavior |

## 2. Task 1 card anatomy

The card is a compact content container. The image is followed by a body containing a title, descriptive paragraph, and primary action link.

Recommended refinements:
- Use a meaningful title element for the page.
- Replace placeholder alt text with an image description.
- Keep CTA semantics honest. Use a button only when an action exists; use a link only when navigation is real.
- Set image aspect ratio and responsive width intentionally.

## 3. Task 2 carousel anatomy

The carousel includes:
- One root element with ID `carouselExampleDark`.
- Three indicator buttons, each with `data-bs-slide-to`.
- Three slide elements, the first marked active.
- Per-slide interval values.
- Previous and next controls.

The indicator target and control target must match the root ID. Indicator indexes must correspond to slide order. Exactly one slide should be active initially.

### Accessibility considerations

- Provide useful alt text for every slide image.
- Provide a heading or context explaining the carousel.
- Ensure controls have accessible labels.
- Avoid unexpectedly moving content. Consider pause controls and reduced-motion preferences when autoplay is used.
- Ensure captions are readable against each image.

## 4. Task 3 navigation and dropdown

The navigation combines a logo, Courses dropdown, placeholder Job Portal/PW Skills Lab links, and Login trigger.

Recommended refinements:
- Use a responsive navbar pattern where appropriate.
- Avoid large inline margin offsets for positioning.
- Ensure menu links have meaningful destinations.
- Maintain keyboard access and visible focus.
- Do not use `href="#"` for non-functional navigation in production.

## 5. Task 3 modal

The modal is targeted by `#exampleModal`. It includes an email field and password field with labels.

The modal's existence does not imply authentication. The Login button in the footer is not wired to a submit handler. If a backend is added later, it must be separately designed and secured.

## 6. Component version consistency

These pages reference Bootstrap 5.3.2. The HTML must keep CSS and JavaScript versions aligned and SRI hashes accurate for the exact files used.
