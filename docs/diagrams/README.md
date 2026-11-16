# 🗺️ Diagram Catalogue

Editable Mermaid source diagrams for this repository are stored here. They are intentionally tied to the current static Bootstrap exercises. No backend, authentication, database, or enrollment architecture is implied.

## Current architecture and workflows

| Diagram | Purpose |
|---|---|
| [system-context.mmd](system-context.mmd) | Static HTML, CDN, local media and browser |
| [page-navigation.mmd](page-navigation.mmd) | Visitor path through the three exercises |
| [asset-loading.mmd](asset-loading.mmd) | Browser asset loading sequence |
| [task-1-card.mmd](task-1-card.mmd) | Course card render and placeholder CTA |
| [task-2-carousel.mmd](task-2-carousel.mmd) | Carousel controls and slide state |
| [task-3-modal.mmd](task-3-modal.mmd) | Dropdown and login modal boundary |
| [dfd-level-0.mmd](dfd-level-0.mmd) | Level 0 data-flow context |
| [dfd-level-1.mmd](dfd-level-1.mmd) | Level 1 browser/component flow |
| [deployment.mmd](deployment.mmd) | Static publishing and validation |
| [test-workflow.mmd](test-workflow.mmd) | Manual QA path |
| [component-map.mmd](component-map.mmd) | Bootstrap component map |

## Design caveats

- The carousel's state is temporary browser component state.
- The modal is visual only, with no authentication handler.
- The enrollment CTA and several navigation anchors are placeholders.
- No database ERD, API sequence, server deployment diagram, or class diagram is included because there are no such application systems in the source.

## Updating diagrams

Change the relevant diagram in the same commit as the HTML change. Keep diagram labels aligned to actual IDs, data attributes, and behavior. GitHub renders Mermaid in supported Markdown contexts.
