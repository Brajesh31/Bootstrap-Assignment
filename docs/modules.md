# 🧩 Modules and File Responsibilities

## Current architecture

The repository does not contain software modules in the package/module-system sense. Each exercise is a standalone HTML document. This page describes logical responsibilities without inventing code modules.

| Logical module | File or directory | Responsibility |
|---|---|---|
| Course card UI | `Task_1.html` | Static course image, title, description and placeholder CTA |
| Carousel UI | `Task_2.html` | Three slides, indicators, timing and navigation controls |
| Navigation UI | `Task_3.html` | Logo, tab-style nav links and dropdown |
| Modal UI | `Task_3.html` | Presentation-only login dialog and form controls |
| Media assets | `media/` | Local images used in page markup |
| Visual references | `output/` | Saved example renders |
| Documentation | `docs/` | Setup, architecture, testing and contributor guidance |
| GitHub automation | `.github/workflows/` | Existing README automation and newly added repository checks |

## External component module

Bootstrap 5.3.2 is loaded remotely. The carousel, dropdown and modal JavaScript behavior is supplied by the Bootstrap bundle. The project does not vendor or modify Bootstrap's source.

## Change impact

| Change | Review |
|---|---|
| Card text or CTA | Task_1.html, features.md, usage.md |
| Carousel slides | Task_2.html, media/, indicators and carousel tests |
| Dropdown links | Task_3.html, components.md, keyboard review |
| Modal structure | Task_3.html, accessibility and security docs |
| Image replacement | media/, alt text, assets.md, asset rights |
| Bootstrap upgrade | all Task HTML files, CDN URLs, SRI values, tests |

## Future organization

If the assignment becomes a larger site, shared templates or components may become useful. Introduce them only when the duplication and maintenance cost justify a build tool. Do not create empty `src/`, `services/`, or `models/` folders to imply they already exist.
