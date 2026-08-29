# Rupal Mishra — portfolio

Static site. No build step, no dependencies, nothing to install.

## Files

- `index.html` — landing page
- `efile.html`, `ecap-care.html`, `calmory.html`, `lok-katha.html`, `instagram-stories.html` — case studies
- `support.js` — the runtime that renders the pages (must sit next to the HTML files)
- `image-slot.js` — image drop component used on the landing page
- `uploads/` — every image the site loads

## Run locally

Any static server works, e.g.:

    npx serve .

Opening `index.html` straight off disk also works.

## Deploy

**Netlify / Vercel / Cloudflare Pages** — drag this whole folder into the dashboard's deploy area, or point the project at a repo containing it. No build command; publish directory is the folder root.

**GitHub Pages** — push the folder contents to a repo, then Settings → Pages → deploy from branch, root.

Anything that serves static files will work. Keep the folder structure intact: `support.js`, `image-slot.js` and `uploads/` are all referenced relatively.

## Custom domain

Point the domain at your host per its docs. Nothing in the code needs changing — all links are relative.

## Editing later

The pages are plain HTML with inline styles. Text lives directly in the markup; the landing page's project list and "things I love" cards are arrays near the bottom of `index.html`.
