# Hero Image Fix Pass — May 2026

## Fixed
- Replaced the homepage hero image reference with relative JPEG paths so it resolves correctly whether the site is served from the domain root or a GitHub Pages project path.
- Added optimized 700px and 1200px JPEG hero derivatives:
  - `assets/images/nathan-anderson-poster-wide-700.jpg`
  - `assets/images/nathan-anderson-poster-wide-1200.jpg`
- Kept the hero image uncropped using the existing `technical-hero-figure` containment rules.
- Converted homepage evidence/card image references to relative paths for the same deployment-path safety.
- Preserved lazy loading for below-fold images and kept the hero image eager/high-priority.

## Why this matters
Absolute `/assets/...` image paths can fail when a GitHub Pages site is deployed under a repository path such as `/future-pfd/`. Relative homepage paths resolve under both `/` and `/future-pfd/`.
