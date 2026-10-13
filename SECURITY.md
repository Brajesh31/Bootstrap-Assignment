# Security Policy

## Scope

This repository is a static front-end exercise. It has no server-side application, API, database, account system, or real authentication flow. The login dialog is a visual demonstration only and must not be used to collect actual passwords. Reports about the example pages, repository dependencies, or unsafe changes to the project are in scope.

## Supported versions

Security fixes are considered for the latest state of the main branch. No older release or deployed service is maintained under this policy.

## Reporting a vulnerability

Please do not publish suspected vulnerabilities in a public issue or pull request. Use GitHub's private vulnerability reporting for this repository if it is enabled: https://github.com/Brajesh31/Bootstrap-Assignment/security/advisories/new. If private reporting is unavailable, contact @brajesh31 through a private channel listed on the GitHub profile.

Include the affected file or page, browser and relevant environment, the impact, and steps to reproduce safely. Redact credentials, personal information, and unrelated sensitive data. Do not probe systems or services that you do not own.

The maintainer will acknowledge reports as reasonably possible, investigate, and coordinate any fix and disclosure with the reporter. There is no guaranteed response time or formal service-level agreement.

## Safe use

The Bootstrap CSS and JavaScript are loaded from jsDelivr with integrity metadata. Keep the integrity value aligned with the exact upstream asset version when changing CDN URLs. Review external resources and contributed images before adding them. Never treat the demo form as a secure login.
