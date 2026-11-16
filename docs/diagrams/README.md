# 🗺️ Diagram Catalogue

The diagrams in this directory are editable Mermaid source files. They describe the current static Bootstrap exercises and their browser interactions.

## 🏗️ Architecture and components

| Diagram | Purpose |
|---|---|
| [system-context.mmd](system-context.mmd) | Static HTML, CDN, local media and browser boundary |
| [component-map.mmd](component-map.mmd) | Card, carousel, navigation, dropdown and modal components |
| [asset-loading.mmd](asset-loading.mmd) | Static asset and CDN loading sequence |

## 🧭 Visitor and task workflows

| Diagram | Purpose |
|---|---|
| [page-navigation.mmd](page-navigation.mmd) | Choose and explore each task |
| [task-1-card.mmd](task-1-card.mmd) | Course card and placeholder CTA |
| [task-2-carousel.mmd](task-2-carousel.mmd) | Carousel slide state |
| [task-3-modal.mmd](task-3-modal.mmd) | Dropdown and login modal boundary |

## 🔄 Engineering and QA workflows

| Diagram | Purpose |
|---|---|
| [dfd-level-0.mmd](dfd-level-0.mmd) | Level 0 data-flow context |
| [dfd-level-1.mmd](dfd-level-1.mmd) | Level 1 browser/component data flow |
| [deployment.mmd](deployment.mmd) | Static publishing |
| [test-workflow.mmd](test-workflow.mmd) | Manual verification process |

## 📌 Diagram scope

No database ERD, API sequence for application endpoints, backend class diagram, or infrastructure topology is included because those systems do not exist in this repository. The login modal is not authentication and the CTA does not enroll a learner.

Update diagrams in the same change as the HTML they describe.

## Extra diagram usage

When adding a new task, include a page-flow diagram only when there is a distinct user journey. Keep source labels consistent with HTML IDs and Bootstrap target selectors. Do not draw database tables or REST endpoints for a static UI exercise.
