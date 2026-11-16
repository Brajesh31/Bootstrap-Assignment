# ADR 0001: Keep the exercises as static pages

- **Status:** Accepted
- **Date:** 2026-11-17

## Context

The repository consists of three independent HTML files and local image assets. There is no package manifest, build tool, framework, or application server.

## Decision

Keep the exercises directly runnable as static HTML. Do not introduce a frontend framework, bundler, or server solely to create a more complex folder structure.

## Consequences

Positive:
- Simple learning experience.
- No build or dependency installation step.
- Easy to preview with a browser or basic static server.
- Each task has a clear scope.

Trade-offs:
- Shared markup can become repetitive.
- More complex interactions may require a deliberate JavaScript or build architecture.
- CDN availability affects Bootstrap behavior.

## Revisit when

A real product requirement makes shared components, routing, dynamic data, or a more structured frontend build genuinely necessary.
