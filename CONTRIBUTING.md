# 🤝 Contributing to Bootstrap Assignment

Thank you for considering a contribution. This repository is a compact educational project demonstrating Bootstrap 5.3.2 through three standalone HTML exercises. Contributions should keep the examples understandable, accessible, and easy to preview.

## 🧭 Before you start

- Read the root [README](README.md) and [documentation hub](docs/README.md).
- Inspect the relevant task page before proposing a change.
- Search existing issues and pull requests.
- Discuss substantial scope changes before introducing frameworks, backend services, or persistent data.
- Do not commit credentials, private data, generated caches, or unrelated editor files.

## 🛠️ Local setup

No Node.js or npm installation is required.

```bash
cd Assignment_14_Bootstrap
python3 -m http.server 8000
```

Open `http://localhost:8000/Task_1.html`, `Task_2.html`, or `Task_3.html`.

## 🧩 Making a change

1. Create a focused branch from `main`.
2. Edit the HTML page responsible for the relevant exercise.
3. Preserve relative media paths or update them consistently.
4. Keep Bootstrap CSS and JS versions aligned.
5. Verify Subresource Integrity hashes if CDN assets change.
6. Use semantic HTML, descriptive page titles, valid labels, and meaningful alt text.
7. Use responsive Bootstrap utilities rather than brittle inline offsets where practical.
8. Do not wire a real authentication system or collect credentials without an approved security design.
9. Update relevant documentation and Mermaid diagrams.
10. Review the final diff and ensure no original asset or exercise was removed unintentionally.

## 🖼️ Images and media

Only contribute images you created or are permitted to redistribute. Record the source, author, license, and attribution requirements. The repository's MIT source-code license does not automatically cover the images in `media/`.

## 🧪 Verification

For Task 1, inspect card layout, image, title and CTA destination.

For Task 2, verify all slides, indicators, timing, previous/next controls, alt text and keyboard operation.

For Task 3, verify dropdown, modal, labels, focus management and placeholder navigation. Confirm that the modal does not imply real authentication.

Across all pages, check:
- Browser console and Network panel.
- Local images and Bootstrap CDN assets.
- Keyboard-only navigation and visible focus.
- Mobile and desktop layout.
- Accurate documentation.

## 📝 Pull request expectations

Include:
- Problem statement and user-facing impact.
- Files and exercise pages changed.
- Bootstrap version/SRI changes, if any.
- Asset additions and rights information.
- Manual verification performed.
- Accessibility, privacy and security considerations.
- Genuine screenshots for visual changes.

## 🔐 Security

Report vulnerabilities privately using [SECURITY.md](SECURITY.md). Do not include passwords, tokens, or exploit details in public issues.

## 🌱 Project conduct

All contributors are expected to follow [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).
