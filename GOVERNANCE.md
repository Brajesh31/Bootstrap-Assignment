# 🏛️ Project Governance

## 1. Purpose

This document explains how changes to Bootstrap Assignment are proposed, reviewed, and maintained. The repository is an educational static HTML project containing three Bootstrap exercises.

## 2. Project stewardship

The repository owner is responsible for:
- Reviewing and accepting changes.
- Maintaining the default branch and repository settings.
- Keeping project scope and documentation accurate.
- Reviewing security reports and dependency changes.
- Protecting repository history and original learning assets.

A contribution does not automatically grant maintainer privileges.

## 3. Decision principles

Changes should be evaluated for learning value, correctness, accessibility, maintainability, security, and consistency with the static educational purpose.

Introducing real authentication, enrollment, payments, APIs, databases, or user data collection requires a separate product and technical design review. Such changes are not ordinary markup updates.

## 4. Contribution review

Pull requests should include the affected task, a concise rationale, manual verification steps, screenshots for visible changes, and any accessibility, security, or asset-licensing impact.

## 5. Architecture decisions

Significant choices should be captured as numbered records in `docs/adr/`. Records should explain context, decision, consequences, and review triggers.

## 6. Release responsibility

A release should be checked in a browser and published as static files. The actual hosting provider is not specified by this repository. Do not assume a deployment workflow exists until one is configured and verified.
