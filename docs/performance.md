# ⚡ Performance Guide

## 1. Current performance profile

The project is a small static HTML assignment. Performance is primarily affected by remote Bootstrap CSS/JavaScript downloads, image file sizes, browser rendering, and layout choices. There is no server rendering, API latency, database query, or custom JavaScript runtime.

## 2. Image optimization

The repository includes local PNG and JPEG images in `media/` and saved output images in `output/`. Optimize images before adding new ones:
- Resize to the largest intended rendered dimensions, not arbitrary camera originals.
- Compress without unacceptable visual degradation.
- Choose modern image formats only when the deployment and browser requirements permit.
- Include width/height or aspect ratio to reduce layout shift.
- Avoid loading output screenshots as page assets unless intentionally required.

## 3. Bootstrap CDN

The pages share Bootstrap assets from jsDelivr. CDN delivery avoids committing framework files but introduces an external request dependency. A local copy may reduce dependency on external network availability, but it transfers update and security maintenance responsibility to the repository.

## 4. Carousel behavior

Automatic slide transitions can affect perceived performance and user comfort. Use intervals that allow visitors to understand the image and provide pause control where appropriate. Large images can dominate transfer size and should be optimized.

## 5. Responsive layout

Use Bootstrap responsive grid and spacing utilities. Avoid large inline offsets, fixed widths, and layout rules that cause horizontal scrolling. Task 3's large inline left margin on the Login button is a specific area to review.

## 6. Measurement

Use browser developer tools or Lighthouse on a real served page. Record page URL, viewport, network condition, browser, test date, transfer size, and Core Web Vitals. No benchmark scores are claimed in this repository.
