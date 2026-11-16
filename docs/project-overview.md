# 🎓 Project Overview

## 1. Purpose

Bootstrap Assignment is a small set of static HTML exercises created to demonstrate common Bootstrap 5.3.2 interface patterns. Each task focuses on a different UI composition and can be opened independently in a browser.

The repository is educational. It demonstrates how to compose Bootstrap classes and data attributes with ordinary HTML, use remote Bootstrap CSS/JavaScript, and load local image files.

## 2. Exercises

| Task | UI objective | Main Bootstrap patterns |
|---|---|---|
| Task 1 | Present a Full Stack Web Development course card | Card, responsive utility classes, button styling |
| Task 2 | Display a rotating collection of three images | Carousel, indicators, timed slides, previous/next controls |
| Task 3 | Build a course-oriented navigation bar | Nav tabs, dropdown, modal, form controls |

## 3. Learning objectives

- Understand the Bootstrap grid and utility-class mindset.
- Use Bootstrap's card component for a compact content block.
- Configure a carousel with indicators, intervals, and controls.
- Use data attributes to activate dropdowns and modals.
- Connect local image files through relative paths.
- Read Bootstrap documentation and use versioned CDN assets.
- Consider accessibility in controls, labels, and alternative text.

## 4. Intended audience

The repository is suitable for students learning frontend development, Bootstrap component composition, HTML structure, browser inspection, and static web hosting. It can also be used as a reference for small isolated UI examples.

## 5. Non-goals

The existing code does not implement:
- User registration, login or identity verification.
- Course enrollment, payment, or learning progress.
- A course catalogue API or server.
- Database storage or session management.
- Admin dashboard or content management.
- Custom application JavaScript.
- A production-ready course platform.

The login modal is a demonstration of Bootstrap's modal UI. Its email/password fields are not submitted to an authentication service. The Enroll Now link uses a placeholder destination.

## 6. Runtime architecture

The browser loads each HTML file and its local media. Bootstrap 5.3.2 CSS and the JavaScript bundle are fetched from jsDelivr. The repository contains no compile or bundling stage.

## 7. Success criteria for the assignment

- Each task page loads successfully.
- All referenced local images resolve.
- Bootstrap styling is available when the CDN is reachable.
- The Task 2 carousel can be operated with indicators and previous/next controls.
- The Task 3 dropdown and modal open and close.
- The page structure remains usable with keyboard navigation.
- The examples are not mistaken for real enrollment or authentication services.
