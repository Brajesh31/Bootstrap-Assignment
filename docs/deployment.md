# Deployment

## Hosting model

The project can be published as static files using any host that serves HTML and image assets. There is no backend process, database, API, build output, or environment configuration.

The repository has no root index.html. Configure the hosting document root to Assignment_14_Bootstrap if you want the three task pages at the site root, or publish the repository and link to the nested files by path. Do not assume a root URL will select a task page automatically.

## Publish contents

Include all three Task HTML files and the complete media directory. The output directory contains saved example renders and is not required for the pages to run. Preserve the folder relationship between each page and media/ so image references continue to work.

No compilation or dependency installation is required. A static host may publish the folder directly. There are no runtime environment variables; .env.example is informational only.

## External dependency and operation

The HTML requests Bootstrap 5.3.2 CSS and the JavaScript bundle from jsDelivr. The host and users need network access to that CDN for styling and interactive components. If the CDN is blocked, the page will not have its intended Bootstrap appearance or interactions. A local Bootstrap bundle can be considered if reliable offline behavior is required, with integrity and version checks updated accordingly.

This repository's login modal is not authentication, and the course action is not enrollment. Do not present the pages as a production login or course registration service. If real credentials or user submissions are ever introduced, that requires a separately designed and secured backend.

Before making the site public, verify that the bundled images may be published and that their third-party rights are documented. The MIT source license does not by itself grant rights to those images.
