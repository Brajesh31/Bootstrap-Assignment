# ▶️ Runbook: Local Preview

## Purpose

Open the three Bootstrap exercises locally without installing a package manager or changing the source.

## Steps

1. Clone the repository.
2. Open a terminal at the repository root.
3. Enter the exercise directory:

   ```bash
   cd Assignment_14_Bootstrap
   ```

4. Start Python's static server:

   ```bash
   python3 -m http.server 8000
   ```

   On Windows, `py -m http.server 8000` is also available when the Python launcher is installed.

5. Open one of:
   - `http://localhost:8000/Task_1.html`
   - `http://localhost:8000/Task_2.html`
   - `http://localhost:8000/Task_3.html`

6. Inspect the browser console and Network panel.
7. Stop the server with Ctrl+C.

## Expected result

The page markup and local images load. Bootstrap styling and interactive components load when the jsDelivr CDN is reachable.

## Troubleshooting

- If images fail, confirm the media directory is next to the HTML files.
- If Bootstrap is missing, check CDN connectivity and SRI errors.
- If the root URL shows a directory listing, open a Task page directly because the repository has no index.html.
