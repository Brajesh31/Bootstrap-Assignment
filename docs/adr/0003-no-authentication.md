# ADR 0003: Login modal is not authentication

- **Status:** Accepted
- **Date:** 2026-11-17

## Context

Task 3 contains a Bootstrap modal with email and password inputs and a Login button. The form has no action URL, submit handler, API, or backend.

## Decision

Treat the modal solely as a visual component exercise. Do not solicit real credentials or advertise account functionality.

## Consequences

- Public documentation must state that login is not implemented.
- No database schema or authentication flow should be invented.
- Any future authentication work requires a separate threat model, backend design, secure password handling, privacy review, and operational owner.
- Static browser files must never contain authentication secrets.

## Revisit when

The project receives an explicit requirement and approved design for a real user identity system.
