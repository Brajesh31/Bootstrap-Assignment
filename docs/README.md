# 📚 Bootstrap Assignment Documentation Hub

Welcome to the documentation for the three Bootstrap 5.3.2 HTML exercises in this repository.

> [!IMPORTANT]
> This is a static educational project. It has no real login, enrollment service, API, database, account system, or backend. The Task 3 modal and Task 1 call-to-action are demonstrations only.

## 🧭 Choose a reading path

- **Understand the project:** [Overview](project-overview.md) → [Features](features.md) → [Usage](usage.md) → [Limitations](limitations.md).
- **Understand the implementation:** [Project structure](project-structure.md) → [Architecture](architecture.md) → [Components](components.md) → [Data flow](data-flow.md) → [Diagrams](diagrams/README.md).
- **Run and verify it:** [Installation](installation.md) → [Configuration](configuration.md) → [Testing](testing.md) → [Manual QA matrix](manual-qa-matrix.md) → [Troubleshooting](troubleshooting.md).
- **Review quality:** [Accessibility](accessibility.md) → [Responsive design](responsive-design.md) → [Browser compatibility](browser-compatibility.md) → [Performance](performance.md).
- **Review safety and rights:** [Security](security.md) → [Privacy](privacy.md) → [Asset rights register](asset-rights-register.md).

## 📖 Documentation catalogue

| Guide | What it covers |
|---|---|
| [Project overview](project-overview.md) | Purpose, audience, learning objectives and non-goals |
| [Features](features.md) | Task 1 card, Task 2 carousel, Task 3 navigation/modal |
| [Usage](usage.md) | How to interact with each page |
| [Project structure](project-structure.md) | Directory tree and file responsibilities |
| [Architecture](architecture.md) | Static HTML, CDN and browser model |
| [System design](system-design.md) | Component boundaries and trust model |
| [Components](components.md) | Bootstrap component breakdown |
| [Modules](modules.md) | Responsibilities of each page and shared asset group |
| [Data flow](data-flow.md) | Browser assets and temporary UI state |
| [API boundary](api.md) | Existing browser attributes and the absence of a server API |
| [Database status](database.md) | Why no persistence layer exists |
| [Diagrams](diagrams/README.md) | Editable Mermaid diagram catalogue |
| [Installation](installation.md) | Direct open and local Python HTTP server |
| [Configuration](configuration.md) | CDN, SRI and carousel configuration |
| [Development](development.md) | Editing and review process |
| [Coding standards](coding-standards.md) | HTML, Bootstrap, images and documentation conventions |
| [Testing](testing.md) | Test strategy and manual verification |
| [Manual QA matrix](manual-qa-matrix.md) | Repeatable test cases and result recording |
| [Browser compatibility](browser-compatibility.md) | Browser families, viewports and compatibility evidence |
| [Accessibility](accessibility.md) | Keyboard, focus, labels and alternative text |
| [Responsive design](responsive-design.md) | Mobile, tablet and desktop verification |
| [Performance](performance.md) | CDN, image and layout performance |
| [Security](security.md) | Login demonstration and CDN trust boundaries |
| [Privacy](privacy.md) | Current data collection and privacy limitations |
| [Assets](assets.md) | Media inventory and asset usage |
| [Asset rights register](asset-rights-register.md) | Provenance, licensing and attribution tracking |
| [Limitations](limitations.md) | Verified missing functionality |
| [Future scope](future-scope.md) | Prioritized improvements |
| [Deployment](deployment.md) | Static hosting guidance |
| [Release process](release-process.md) | Pre-release and rollback checklist |
| [Maintenance](maintenance.md) | Routine upkeep |
| [Observability](observability.md) | Static-host monitoring considerations |
| [FAQ](faq.md) | Common questions |
| [Troubleshooting](troubleshooting.md) | CDN, paths and component issues |
| [Glossary](glossary.md) | Technical terminology |
| [References](references.md) | Official Bootstrap and web references |
| [Architecture decisions](adr/README.md) | Recorded decisions and rationale |
| [Runbooks](runbooks/README.md) | Local preview, asset verification and publishing |

## 🔎 Verified source inventory

| Source | Purpose |
|---|---|
| Assignment_14_Bootstrap/Task_1.html | Course card |
| Assignment_14_Bootstrap/Task_2.html | Three-image carousel |
| Assignment_14_Bootstrap/Task_3.html | Navigation, dropdown and login modal |
| Assignment_14_Bootstrap/media/ | Images used by the task pages |
| Assignment_14_Bootstrap/output/ | Saved example renders |
| .github/workflows/ | Static checks, documentation checks, security scan and README maintenance |

## 🛠️ Keeping documentation accurate

When markup, Bootstrap versions, media paths, or interactions change:

1. Update the relevant page guide and project structure.
2. Update affected Mermaid diagrams.
3. Recheck Subresource Integrity values and local asset references.
4. Run automated repository checks and the applicable manual QA cases.
5. Record browser and accessibility results only after testing.
6. Keep current behavior separate from proposed future functionality.
7. Review asset provenance before redistributing new or changed media.

Do not add fabricated API/database schemas, invented test results, or screenshots that were not captured from the actual pages.
