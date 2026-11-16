# 📚 Bootstrap Assignment Documentation Hub

Welcome to the engineering and learning documentation for this repository. It contains three static Bootstrap exercises: a course card, a carousel, and a navigation/dropdown/login-modal layout.

> [!IMPORTANT]
> This repository is a front-end assignment, not a production course platform. The login modal is only a visual form, the enrollment link is a placeholder, and the navigation links do not connect to working services. No API, database, authentication system, backend, or build pipeline is included.

## 🧭 Recommended reading paths

- **New learner:** [Project Overview](project-overview.md) → [Exercises](features.md) → [Usage](usage.md) → [Limitations](limitations.md).
- **Frontend developer:** [Installation](installation.md) → [Project Structure](project-structure.md) → [Architecture](architecture.md) → [Bootstrap Components](components.md) → [Testing](testing.md).
- **Quality reviewer:** [Accessibility](accessibility.md) → [Security](security.md) → [Performance](performance.md) → [Deployment](deployment.md).
- **Contributor:** [Development](development.md) → [Coding Standards](coding-standards.md) → [Contribution Guide](../CONTRIBUTING.md).

## 📖 Documentation catalogue

| Category | Document | Coverage |
|---|---|---|
| Product | [Overview](project-overview.md) | Assignment purpose, scope, audience and non-goals |
| Product | [Features](features.md) | Task 1, Task 2 and Task 3 behavior |
| Product | [Usage](usage.md) | How to open and interact with the pages |
| Product | [Limitations](limitations.md) | Placeholder links and missing services |
| Structure | [Project Structure](project-structure.md) | File tree, assets and output screenshots |
| Structure | [Assets](assets.md) | Media inventory, dimensions and attribution workflow |
| Architecture | [Architecture](architecture.md) | Static HTML and CDN model |
| Architecture | [System Design](system-design.md) | Component boundaries and trust model |
| Architecture | [Data Flow](data-flow.md) | Browser, Bootstrap and form boundary |
| Architecture | [Workflow](workflow.md) | Page loading and interaction sequences |
| UI | [Components](components.md) | Card, carousel, nav, dropdown and modal |
| UI | [Responsive Design](responsive-design.md) | Viewport behavior and layout review |
| Setup | [Installation](installation.md) | Direct open and Python static server |
| Setup | [Configuration](configuration.md) | No build configuration, CDN version and SRI |
| Development | [Development](development.md) | Editing and review workflow |
| Development | [Coding Standards](coding-standards.md) | HTML and Bootstrap practices |
| Quality | [Testing](testing.md) | Manual browser test matrix |
| Quality | [Accessibility](accessibility.md) | Keyboard, labels, alt text and contrast |
| Quality | [Performance](performance.md) | Images, CDN and network cost |
| Quality | [Security](security.md) | Credential and dependency boundaries |
| Privacy | [Privacy](privacy.md) | No current data collection |
| Operations | [Deployment](deployment.md) | Static publishing |
| Operations | [Release Process](release-process.md) | Review checklist |
| Operations | [Maintenance](maintenance.md) | Routine upkeep |
| Operations | [Runbooks](runbooks/README.md) | Preview, asset audit and release |
| Reference | [API](api.md) | Explicit absence of backend endpoints |
| Reference | [Database](database.md) | No persistence layer |
| Reference | [FAQ](faq.md) | Common questions |
| Reference | [Troubleshooting](troubleshooting.md) | CDN, images and Bootstrap interactions |
| Reference | [Glossary](glossary.md) | Bootstrap and web terminology |
| Reference | [References](references.md) | Official Bootstrap and web standards |
| Governance | [ADRs](adr/README.md) | Architecture decisions |

## 🔎 Source inventory

| Path | Purpose |
|---|---|
| `Assignment_14_Bootstrap/Task_1.html` | Course card |
| `Assignment_14_Bootstrap/Task_2.html` | Three-image Bootstrap carousel |
| `Assignment_14_Bootstrap/Task_3.html` | Navigation, dropdown and login modal |
| `Assignment_14_Bootstrap/media/` | Images referenced by the HTML exercises |
| `Assignment_14_Bootstrap/output/` | Saved example renders, not runtime dependencies |
| `docs/` | Project documentation |
| `.github/workflows/update-readme.yml` | Existing README automation, preserved |

## 🧩 Diagram catalogue

Editable Mermaid diagrams live in [diagrams/](diagrams/README.md). They describe the static page architecture, browser loading, task-specific user journeys, carousel state, modal boundary, asset delivery and deployment.

## ✅ Documentation maintenance rules

1. Keep file and asset paths aligned with the actual repository tree.
2. Use accurate descriptions of Bootstrap's actual component behavior.
3. Keep future backend proposals separate from the current implementation.
4. Do not publish fabricated screenshots or unverified external demo links.
5. Check image rights before reuse. The root MIT license does not automatically cover third-party media.
6. Update diagrams and documentation whenever the HTML or Bootstrap version changes.
