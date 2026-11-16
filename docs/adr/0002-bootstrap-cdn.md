# ADR 0002: Use Bootstrap from jsDelivr

- **Status:** Accepted
- **Date:** 2026-11-17

## Context

Each page references Bootstrap 5.3.2 CSS and JavaScript from jsDelivr with integrity and crossorigin metadata. No local Bootstrap distribution is stored in the repository.

## Decision

Retain the existing CDN approach for the educational assignment. Keep CSS and JavaScript versions aligned and verify SRI values when changing exact files.

## Consequences

Positive:
- No framework distribution is committed.
- The project remains small.
- Bootstrap assets are centrally delivered.

Trade-offs:
- Styling and JavaScript interactions depend on network/CDN availability.
- Version upgrades require careful SRI updates.
- Third-party request behavior should be reviewed for privacy and hosting expectations.

## Revisit when

Offline operation, supply-chain policy, or host constraints justify a local Bootstrap distribution.
