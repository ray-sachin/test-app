# Simple Web App with About Page and Stylesheet

## Overview
This is a lightweight multi-page web app consisting of:
- Home page (index.html)
- About page content (about.html, loaded dynamically or opened directly)
- A shared stylesheet (styles.css) for consistent appearance

The app uses hash-based routing to dynamically load the About page content from about.html into the main layout, keeping styling and navigation consistent. A direct link to open about.html as a standalone page is also provided.

## Setup
1. Ensure the following files are in the same directory:
   - index.html (this file)
   - about.html (provided in repo)
   - styles.css (provided in repo)
   - LICENSE (if not present, add one appropriate for your project)

2. Serve the directory with a static web server to enable dynamic loading via fetch:
   - Using Node.js: npx serve .
   - Using Python 3: python -m http.server 8000
   - Or open with any static server of your choice

Note: Opening index.html directly from the file system may prevent fetch from loading about.html due to browser security policies. Using a local server is recommended.

## Usage
- Visit the Home page at http://localhost:PORT/index.html
- Click “About” in the navigation to view the About content within the main layout.
- Alternatively, click “Open About (standalone)” to open about.html directly in a new tab.

## Improvements from Previous Version (Round 2 -> Round 3)
- Added a dedicated About page (about.html) and integrated it via a simple client-side router.
- Introduced an external CSS stylesheet (styles.css) for consistent typography and background styling across pages.
- Implemented a top navigation bar with active-link indication and accessibility improvements (skip link, focus management, aria-current).
- Provided a graceful fallback to open About as a standalone page if dynamic loading is blocked.