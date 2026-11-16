# 🔐 Security Guide

## 1. Current threat boundary

The repository contains static HTML pages, local image assets, and Bootstrap assets loaded from jsDelivr. There is no backend, account system, database, authentication endpoint, enrollment endpoint, or server-side code.

## 2. Never collect real credentials

Task 3 displays email and password fields in a modal, but no form handler or authentication service is implemented. Do not use the modal for real login. Do not ask contributors or visitors to enter their real passwords.

## 3. CDN and Subresource Integrity

Bootstrap is loaded from jsDelivr with SRI and crossorigin attributes. SRI helps the browser verify that the downloaded asset matches the expected hash. When changing versions or filenames:
- Use the official Bootstrap distribution.
- Calculate/copy the integrity hash for the exact file.
- Keep CSS and JS versions aligned.
- Confirm requests are not blocked by integrity errors.
- Review third-party availability and privacy impact.

## 4. Client-side trust

All HTML, markup and client-visible configuration is public. Do not place secrets, API keys, passwords or database credentials in the repository's static pages. The .env.example file does not make a static browser environment private.

## 5. Asset provenance and licensing

The root MIT license applies to project code under its terms. It does not automatically grant reuse rights for all images. Verify the source, owner, license, and permitted reuse of each media file before redistribution.

## 6. Future login/enrollment implementation

A real user service requires server-side authentication and authorization, secure password handling, rate limiting, CSRF protections where relevant, secure session management, input validation, privacy disclosures, retention and deletion rules, and incident response. Never implement credential verification solely in browser JavaScript.

## 7. Reporting a vulnerability

Use the private reporting channel described in the root SECURITY.md. Provide affected file, impact, reproduction steps and safe evidence. Never publish passwords, tokens, or real user information in a public issue.
