# 🔐 Security Policy

## 1. Project scope

Bootstrap Assignment is a static front-end learning project. It contains HTML pages, local media, and Bootstrap 5.3.2 resources loaded from jsDelivr.

It does **not** contain a server-side application, API, database, account service, or real authentication flow. The Task 3 login dialog is a visual demonstration only.

## 2. Supported versions

Security fixes and repository-level changes are considered for the latest state of the `main` branch. No older deployed service or release line is maintained under this policy.

## 3. Reporting a vulnerability

Please do not publish suspected vulnerabilities in a public issue or pull request.

Use GitHub's private vulnerability reporting for this repository when enabled:

[Report a private vulnerability](https://github.com/Brajesh31/Bootstrap-Assignment/security/advisories/new)

If private reporting is unavailable, contact the repository owner through the private channel listed on the GitHub profile.

Include:
- Affected file, page, dependency or workflow.
- Impact and preconditions.
- Steps to reproduce safely.
- Browser and relevant environment.
- Suggested mitigation, if known.

Redact credentials, personal information, tokens and unrelated sensitive data. Do not probe systems you do not own.

## 4. Response expectations

The project is maintained on a best-effort basis. The maintainer will assess reports, ask for clarification when needed, and coordinate fixes or disclosure. No response-time SLA is promised.

## 5. Safe use of the current demo

- Never enter real passwords in the login modal.
- Do not describe the modal as an authentication system.
- Do not place API keys, tokens or credentials in public HTML.
- Do not add form submission or tracking without an explicit privacy and security review.
- Verify asset provenance before distribution.

## 6. CDN security

Bootstrap CSS and JavaScript are loaded from jsDelivr with integrity metadata. When changing a URL or version:
1. Use official upstream files.
2. Obtain the SRI hash for the exact file.
3. Keep CSS and JavaScript versions aligned.
4. Confirm the browser reports no integrity error.
5. Review the upstream release notes.

## 7. Future authentication

If real authentication or enrollment is introduced, it needs a separately designed server-side service, secure password handling, session management, rate limiting, abuse protection, privacy disclosures, retention/deletion policy, monitoring and incident response. Client-side HTML alone cannot securely authenticate users.
