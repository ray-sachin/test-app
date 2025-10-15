# Simple Web App (Home & About)

## Overview
This is a minimal single-page web app that includes:
- A Home page
- A new About page
- A CSS stylesheet (inline) derived from the provided styles.css

Navigation is hash-based, so the app works entirely as a single `index.html` without a build step or server.

## Setup
No installation is required.

Options to run:
- Double-click `index.html` to open it in your browser.
- Or serve it locally (recommended for consistent hash routing):
  - Using Python 3: `python -m http.server 8080`
  - Using Node (http-server): `npx http-server -p 8080`

Then open http://localhost:8080 in your browser.

## Usage
- Click “Home” or “About” in the navigation bar to switch between views.
- You can deep link directly:
  - Home: `#/`
  - About: `#/about`
- The stylesheet is embedded in a `<style>` block to keep the app self-contained, using the provided `styles.css` baseline:
  - `body { font-family: Arial; background-color: #f0f0f0; }`

Notes:
- The About page content matches the provided `about.html` snippet.
- Since this deliverable is constrained to a single HTML file output, the CSS is inlined for portability.