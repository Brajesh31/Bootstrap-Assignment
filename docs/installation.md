# Installation and preview

## Requirements

- A modern desktop or mobile web browser.
- Internet access if you want Bootstrap's CDN styling and interactive components.
- A static file server is optional. Python 3 includes a simple local server, but the pages do not require Python to open.

There is no package manager manifest, build step, application server, environment configuration, or database to install.

## Open a page directly

From the repository, open one of these files in your browser:

- Assignment_14_Bootstrap/Task_1.html
- Assignment_14_Bootstrap/Task_2.html
- Assignment_14_Bootstrap/Task_3.html

The pages reference media with relative paths, so keep each HTML file beside the media directory. If a page is moved by itself, its images will no longer resolve.

## Serve over local HTTP

Serving the pages over HTTP can make browser inspection more representative. In PowerShell:

~~~powershell
cd Assignment_14_Bootstrap
py -m http.server 8000
~~~

If the py launcher is unavailable, use python -m http.server 8000. On macOS or Linux, use:

~~~sh
cd Assignment_14_Bootstrap
python3 -m http.server 8000
~~~

Open http://localhost:8000/Task_1.html, http://localhost:8000/Task_2.html, or http://localhost:8000/Task_3.html. Stop the server with Ctrl+C when finished.

## Bootstrap assets

The page sources reference Bootstrap 5.3.2 CSS and JavaScript on jsDelivr. A network connection is needed to load them. The local images remain in media/. Bootstrap is not vendored in this repository; offline use requires an intentional change to bundle the Bootstrap files locally and keep the version and integrity metadata correct.

## No environment setup

The project reads no environment variables. .env.example records that no local settings or secrets are needed.
