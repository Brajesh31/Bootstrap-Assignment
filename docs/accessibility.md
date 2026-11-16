# ♿ Accessibility Guide

## 1. Purpose

The three exercises should remain understandable and operable by visitors using keyboards, screen readers, zoom, and different input methods. Bootstrap provides useful component patterns, but the page markup still determines content semantics and accessible names.

## 2. Document structure

- Use an informative page title instead of the generic title `Document`.
- Maintain a logical heading sequence.
- Use semantic landmarks where the page has meaningful navigation and main content.
- Keep link text descriptive.
- Do not use a placeholder link as a functional action.

## 3. Images and alternative text

The task pages currently contain placeholder alt text such as `...`. Replace each with a concise description of the image's relevant content. If an image is purely decorative and conveys no information, use an empty alt value rather than meaningless text.

## 4. Carousel accessibility

The carousel rotates automatically and contains indicator and previous/next controls. Review:
- Whether automatic rotation is necessary.
- Whether visitors can pause or stop the rotation.
- Whether controls have descriptive accessible names.
- Whether the active slide state is conveyed.
- Whether text captions contrast with each image.
- Whether keyboard users can operate all controls.
- Whether slide changes are too frequent for the content.

## 5. Navigation and dropdown

- Ensure all links have meaningful labels and destinations.
- Keep keyboard focus visible.
- Verify dropdown activation and dismissal via keyboard.
- Avoid using anchors with `href="#"` for actions.
- Use a responsive navigation pattern that remains usable at narrow widths.

## 6. Modal and form accessibility

The modal includes email and password inputs with labels. Verify that focus enters the modal, remains appropriately managed while open, and returns to the trigger when closed. Ensure escape/close behavior matches Bootstrap's intended behavior.

The login form is not functional. Do not collect real credentials. A future real authentication service would need accessible validation and error feedback as well as the relevant security controls.

## 7. Visual accessibility

- Check text and UI contrast.
- Do not convey state through color alone.
- Ensure touch targets are large enough.
- Avoid fixed spacing that breaks at zoom or mobile widths.
- Respect reduced-motion preferences for non-essential effects.

## 8. Verification

Use keyboard-only navigation, browser zoom, screen-reader spot checks, automated accessibility tools, and manual review. Do not claim WCAG conformance without a formal assessment.
