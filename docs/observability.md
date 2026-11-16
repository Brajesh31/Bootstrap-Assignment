# 📊 Monitoring and Observability

## Current state

This repository is static HTML and media. It does not contain server-side logs, application metrics, tracing, or health endpoints. Hosting-level uptime, TLS, and access logs belong to the actual static hosting provider, which is not specified in this repository.

## Useful checks for a hosted copy

- Page availability and HTTP status.
- TLS certificate validity.
- Missing HTML, CSS, JS and image resources.
- CDN availability and Bootstrap integrity errors.
- Browser errors reported through an approved support channel.
- Page loading and responsive behavior.

## Privacy boundary

Do not introduce analytics or visitor tracking without documenting the purpose, data collected, consent expectations, retention and provider. Do not log passwords or form contents.

## Future service monitoring

A future backend would need error rates, latency, availability targets, alerts, structured logs, access controls and an incident escalation owner. That scope is not part of the current assignment.
