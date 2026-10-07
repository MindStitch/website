# mindstitch.dev

Landing site for MindStitch: home page, Terms, Privacy, Refund Policy, 404 and `security.txt`.
Plain static files: no build step, no cookies, no analytics, no third-party requests (fonts are self-hosted in `/fonts`, SIL OFL).

## Deploy

Hosted on Vercel (project `mindstitch`), connected to this repo. Every push to `main` deploys to production.
Vercel settings: Framework Preset **Other**, no build command, output directory `.`.

## Before Paddle reviews the site

- Fill the yellow `[placeholders]` in `terms.html` and `privacy.html` once the company is registered.
- Remove the "Draft" boxes after a lawyer has reviewed the legal pages.
- `/.well-known/security.txt` expires 2027-10-01. Renew the date before then.

## Brand

Navy `#0F162F`, navy-2 `#1A1E51`, indigo `#443CD9`, lavender `#7A81F9`, coral `#FB654C`, white `#FCFCFC`. Font: Outfit; code: JetBrains Mono.
