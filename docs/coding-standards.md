# 📐 Coding Standards

## HTML structure

- Include a valid HTML5 doctype.
- Set the document language.
- Use a descriptive page title.
- Include charset and viewport metadata.
- Prefer semantic headings, navigation landmarks, lists and buttons.
- Keep IDs unique and synchronize `data-bs-target` references.
- Use anchors for navigation and buttons for actions.
- Associate every form label with its input.

## Bootstrap conventions

- Keep the CSS and JS version aligned.
- Use only official Bootstrap component patterns for the selected version.
- Verify SRI hashes when CDN file versions change.
- Use responsive utilities instead of large inline positioning offsets.
- Avoid duplicate or conflicting component attributes.

## Images

- Preserve the `media/` path relationship.
- Use descriptive filenames.
- Add accurate alternative text.
- Keep image provenance and rights documented.
- Optimize file size before adding large assets.

## Accessibility

- Maintain visible focus.
- Ensure keyboard operation.
- Do not use color as the only status indicator.
- Consider reduced motion.
- Ensure modal and carousel controls have meaningful accessible names.

## Documentation

- Use consistent Markdown heading hierarchy.
- Use emojis meaningfully to improve scanning.
- Add diagrams only when they describe a real workflow or explicitly labelled future design.
- Do not invent APIs, databases, test results, deployment URLs or functionality.
