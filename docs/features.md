# ✨ Exercise and Feature Catalogue

This catalogue explains what each HTML task demonstrates and records the current behavioral boundary.

## 🧩 Task 1: Course card

**Source:** `Assignment_14_Bootstrap/Task_1.html`

The page displays a centered Bootstrap card with a local course image, a Full Stack Web Development title, a short MERN-stack description, and a primary Enroll Now anchor.

### Component breakdown

| Element | Purpose |
|---|---|
| `card` | Provides a bordered card container |
| `card-img-top` | Places the course image at the top |
| `card-body` | Groups the heading, description and action |
| `card-title` | Displays course title |
| `card-text` | Displays course summary |
| `btn btn-primary` | Styles the enrollment call-to-action |

### Current limitation

The Enroll Now anchor uses `href="#"`. It does not navigate to an enrollment workflow, process a registration, or collect payment. The image has placeholder alt text and should receive an accurate description.

## 🎞️ Task 2: Image carousel

**Source:** `Assignment_14_Bootstrap/Task_2.html`

The page contains a Bootstrap carousel configured with three local images. It includes three indicators, a 10-second first-slide interval, a 2-second second-slide interval, and previous/next controls.

### Component breakdown

| Element | Purpose |
|---|---|
| `carousel` | Carousel root |
| `carousel-indicators` | Selects a slide directly |
| `carousel-inner` | Wraps all slides |
| `carousel-item` | One slide in the carousel |
| `data-bs-interval` | Controls the slide interval in milliseconds |
| `carousel-control-prev` | Moves to the previous slide |
| `carousel-control-next` | Moves to the next slide |

The Bootstrap JavaScript bundle drives the carousel. The local images are loaded from `media/`.

### Current limitations

- Image alt values are placeholders.
- Captions are empty.
- The carousel has no explicit accessible heading or descriptive context.
- Autoplay may be distracting for some users. Consider a pause mechanism or disable automatic rotation when accessibility requirements call for it.

## 🧭 Task 3: Navigation, dropdown and login modal

**Source:** `Assignment_14_Bootstrap/Task_3.html`

The page demonstrates a tab-style navigation list with a local logo, a Courses dropdown, placeholder Job Portal and PW Skills Lab links, and a Login button that opens a Bootstrap modal.

### Dropdown

The Courses anchor uses `data-bs-toggle="dropdown"` and reveals a list of placeholder menu items when Bootstrap JavaScript is available.

### Modal

The Login button targets `#exampleModal`. The modal includes:
- A dialog title.
- Close button.
- Email input with label and helper text.
- Password input with label.
- Footer Close and Login buttons.

### Current limitation

The modal form has no action URL or submit handler. The footer Login button is not wired to a form submission or authentication API. Never use real credentials in this demonstration.

## 🚫 Cross-project non-features

No API, backend, database, account system, course enrollment, payment, LMS, user session, or application analytics are present in the repository.
