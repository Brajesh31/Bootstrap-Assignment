# 🛠️ Development Guide

## 1. Project workflow

The repository is designed for direct HTML editing. There is no package manager manifest, bundler, custom JavaScript source file, or local Bootstrap build.

## 2. Page ownership

| File | Change when |
|---|---|
| `Assignment_14_Bootstrap/Task_1.html` | Editing course card structure/content |
| `Assignment_14_Bootstrap/Task_2.html` | Editing carousel slides, timing or controls |
| `Assignment_14_Bootstrap/Task_3.html` | Editing nav, dropdown or modal |
| `Assignment_14_Bootstrap/media/` | Adding or replacing referenced images |
| `Assignment_14_Bootstrap/output/` | Updating saved reference renders |
| `docs/` | Updating project and engineering guidance |

## 3. HTML conventions

- Keep `<!DOCTYPE html>` and `lang="en"`.
- Include charset and viewport metadata.
- Use a meaningful page title rather than the generic Document title.
- Use semantic headings and landmarks where appropriate.
- Give images meaningful alternative text.
- Keep labels connected to form controls.
- Use unique IDs and match every `data-bs-target` to a real element.
- Use native anchors for navigation and buttons for actions.

## 4. Bootstrap conventions

- Keep Bootstrap CSS and JavaScript versions aligned.
- Verify SRI values against the exact CDN files.
- Use Bootstrap's documented component markup.
- Match each carousel indicator to a slide.
- Match every modal trigger to the modal's ID.
- Avoid overriding Bootstrap with brittle inline styles when responsive utility classes can express the layout.

## 5. Image handling

- Preserve relative path relationship between HTML and `media/`.
- Use descriptive filenames for newly added assets.
- Optimize large images while preserving intended visual quality.
- Add real alt text based on image content.
- Record source, author and license for third-party media.
- Keep output screenshots separate from runtime assets.

## 6. Manual verification

Open each changed page in a browser. Check:
- Layout and text wrapping.
- Local images.
- CDN availability and browser console.
- Carousel navigation and timing.
- Dropdown and modal behavior.
- Keyboard-only navigation and focus.
- Narrow/mobile and desktop widths.

## 7. Pull request expectations

Explain the task page affected, markup changes, Bootstrap version/SRI changes, assets added, tests performed, and any accessibility or security impact. Include genuine before/after screenshots for visible changes.

## 8. Avoid unnecessary tools

Do not add Node.js, a framework, backend, database, or test package unless a specific need exists. Keep the assignment lightweight and reproducible.
