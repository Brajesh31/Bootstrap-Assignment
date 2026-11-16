# 🗂️ Project Structure

## 1. Repository tree

```text
Bootstrap-Assignment/
├── .github/
│   └── workflows/
│       └── update-readme.yml
├── Assignment_14_Bootstrap/
│   ├── Task_1.html
│   ├── Task_2.html
│   ├── Task_3.html
│   ├── media/
│   │   ├── 1681225007-6197.png
│   │   ├── 64a514966977cc6e87e27504.png
│   │   ├── 653b999fd85a4d9660adf574.png
│   │   ├── 6568179250c244fbec73aaf4.jpg
│   │   └── 6569744750c244a030749278.jpg
│   └── output/
│       ├── task_1.png
│       ├── task_2.png
│       ├── task_3_a.png
│       └── task_3_b.png
├── docs/
│   ├── adr/
│   ├── diagrams/
│   ├── runbooks/
│   └── project and engineering guides
├── .editorconfig
├── .env.example
├── .gitattributes
├── .gitignore
├── CHANGELOG.md
├── CITATION.cff
├── CODEOWNERS
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── README.md
├── ROADMAP.md
├── SECURITY.md
└── SUPPORT.md
```

## 2. Application files

| Path | Role | Notes |
|---|---|---|
| `Task_1.html` | Course card example | Uses one local image |
| `Task_2.html` | Image carousel example | Uses three local images and Bootstrap data attributes |
| `Task_3.html` | Navigation/dropdown/modal example | Uses local logo and a presentation-only login form |
| `media/` | Source image files | Required by relative paths in the task pages |
| `output/` | Saved output images | Reference renders, not loaded by the HTML |

## 3. Repository support files

| File | Responsibility |
|---|---|
| `.editorconfig` | Editor consistency |
| `.env.example` | Documents absence of runtime configuration |
| `.gitattributes` | Git text and line-ending behavior |
| `.gitignore` | Local generated and editor files |
| `README.md` | Project landing page |
| `CHANGELOG.md` | Repository change history |
| `CITATION.cff` | Citation metadata |
| `CODEOWNERS` | Code ownership rules |
| `CODE_OF_CONDUCT.md` | Community conduct |
| `CONTRIBUTING.md` | Contribution workflow |
| `LICENSE` | Existing MIT license |
| `ROADMAP.md` | Planned improvements |
| `SECURITY.md` | Security reporting policy |
| `SUPPORT.md` | Support guidance |

## 4. Runtime dependency model

Bootstrap CSS and JavaScript are loaded remotely from jsDelivr. The local media files are requested relative to each HTML file. There is no package manager manifest or build output.

## 5. Why no backend folders are included

There are no real services, models, routes, tests, or database migrations in the source. Empty `backend/`, `api/`, `database/`, or `tests/` directories would misrepresent the assignment. Add them only when implementation exists.
