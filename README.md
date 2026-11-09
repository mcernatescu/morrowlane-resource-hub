# Morrowlane Resource Hub

A three-page, static **fictional training prototype** for the Vibe Coding Module 2 assignment. All seven documents are invented, non-sensitive sample materials and are **not official Morrowlane policies**.

## Pages

- `index.html` — homepage
- `operations.html` — four operations documents
- `clients.html` — three client documents

## Documents

Six PDFs and one editable Word template live in `resources/`. Every file is marked **SAMPLE - TRAINING USE ONLY**, version 1.0, sample date November 9, 2026.

## Run locally

Open `index.html` in a browser. The relative navigation and download links work without a build tool. Alternatively serve this folder with `python -m http.server 8000` and visit `http://localhost:8000`.

## Update a resource

1. Replace the file under `resources/` (or add a new safe training document).
2. Edit the corresponding resource card in `operations.html` or `clients.html`: title, summary, version, date, file type, and relative download href.
3. Test its link locally and after publishing. Do not use real client data, contracts, credentials, or security procedures.

## Deploy to Netlify

**Quick manual deploy:** Sign in to Netlify, add a site using manual deploy, and drag the extracted `morrowlane-resource-hub` folder (not its parent directory) into the upload area. Netlify serves `index.html` automatically.

**GitHub-based deploy:** Create a GitHub repository, upload the contents of this folder to the root, then connect the repository in Netlify. Build command: leave blank. Publish directory: `.`. Re-deploy after commits.

## Privacy and indexing

The site is public and **does not provide authentication**. Do not publish confidential content. Each HTML page has `<meta name="robots" content="noindex, nofollow">`. `robots.txt` deliberately permits crawler access so crawlers can read that noindex directive; blocking the same pages with `Disallow: /` may prevent crawlers from seeing it. There is no public sitemap. This is not a security boundary: anyone with the URL can access it. The published `robots.txt` can be checked at `<your-netlify-url>/robots.txt`.

## QA before submission

Open all three pages at desktop/tablet/mobile sizes, test all seven downloads and Word editability, keyboard navigation, and confirm the public URL is accessible without login. Use the course stranger test to ensure nothing sensitive appears in the pages or published documents.
