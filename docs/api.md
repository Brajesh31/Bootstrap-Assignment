# 🔌 API and Browser Interface Reference

## 1. Server API status

There is no application HTTP API in this repository. No routes, controllers, GraphQL schema, JSON service, API authentication, request validation, or server process is present.

## 2. Static page catalogue

| Page | Main behavior | Data/network behavior |
|---|---|---|
| `Task_1.html` | Course card | Static HTML and local image; action link is `#` |
| `Task_2.html` | Bootstrap carousel | Static HTML, local images, Bootstrap CDN plugin |
| `Task_3.html` | Dropdown and login modal | Static HTML, Bootstrap CDN plugins; modal form has no handler |

## 3. Bootstrap component interfaces

Bootstrap components are configured through documented data attributes rather than custom repository API functions.

| Component | Attribute pattern | Target |
|---|---|---|
| Carousel | `data-bs-target`, `data-bs-slide`, `data-bs-slide-to` | `#carouselExampleDark` |
| Dropdown | `data-bs-toggle="dropdown"` | Associated dropdown menu |
| Modal | `data-bs-toggle="modal"`, `data-bs-target` | `#exampleModal` |
| Modal dismissal | `data-bs-dismiss="modal"` | Current modal instance |

These are Bootstrap browser component interfaces. They are not project-owned server endpoints.

## 4. Login form boundary

The Task 3 modal contains email and password fields. The form has no action URL or submit handler; the footer Login control is not connected to authentication. It does not verify identity, create a session, transmit credentials, or persist account data.

Never enter real credentials into this demonstration.

## 5. Future API requirements

If an actual login or enrollment service is added, document endpoint method/path, request and response schemas, authentication, authorization, rate limits, validation, error responses, logging, and personal-data handling. Keep secrets server-side and never call a privileged API directly from a public static page.
