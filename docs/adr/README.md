# 🧠 Architecture Decision Records

Architecture Decision Records (ADRs) document important technical choices, their rationale, and the conditions under which they should be revisited.

## Status labels

- **Accepted**: current project decision.
- **Proposed**: awaiting review.
- **Superseded**: replaced by a later decision.
- **Deprecated**: no longer recommended.

## Current records

| ADR | Decision | Status |
|---|---|---|
| [0001 Static pages](0001-static-pages.md) | Keep each exercise as a directly runnable HTML page | Accepted |
| [0002 Bootstrap CDN](0002-bootstrap-cdn.md) | Use a consistent Bootstrap 5.3.2 CDN dependency with integrity metadata | Accepted |
| [0003 No real authentication](0003-no-authentication.md) | Treat the login modal as UI only, never as authentication | Accepted |

Add a new numbered ADR when a change affects structure, dependencies, security, hosting, or long-term maintainability. Do not rewrite a historical decision silently; supersede it when the project direction changes.
