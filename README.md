# Defending the 2026 Election — Field Guide

A single-file static website. No build step, no dependencies, no framework. Just `index.html`.

## Hosting it for free (pick one — easiest first)

### Option 1: Netlify Drop (60 seconds, no account needed at first)
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag `index.html` (or the folder containing it) onto the page
3. You get a live URL instantly (e.g. `https://lucky-name-12345.netlify.app`)
4. Optional: create a free account to claim the site, set a custom subdomain, or attach your own domain

### Option 2: Cloudflare Pages (5 minutes, more permanent)
1. Sign up free at [pages.cloudflare.com](https://pages.cloudflare.com)
2. Click "Upload assets"
3. Upload `index.html`
4. Get a `*.pages.dev` URL with free SSL and a global CDN

### Option 3: GitHub Pages (10 minutes, version controlled)
1. Create a free GitHub account if you don't have one
2. Create a new public repository (any name, e.g. `defending-2026`)
3. Upload `index.html` to the repo
4. Settings → Pages → Source: `main` branch, root → Save
5. Wait ~1 minute, your site is live at `https://yourusername.github.io/defending-2026/`
6. Edits push live by editing the file in GitHub directly — no terminal needed

### Option 4: Vercel (similar to Netlify)
1. Sign up free at [vercel.com](https://vercel.com)
2. Import a Git repo or drag-and-drop
3. Live in seconds

## Custom domain (optional, ~$10–15/year)

Buy a domain at Namecheap, Cloudflare Registrar (cheapest), or Porkbun. Point its DNS at your host (each platform has a one-page guide). Something like `defend2026.org` is memorable.

## Editing the page

Open `index.html` in any text editor (VS Code, Notepad, even TextEdit). The structure is:
- **Header** — top of file, the title and intro paragraphs
- **Trackers** — `<section id="track">`, each tracker is an `<a class="tracker">`
- **Actions** — `<section id="act">`, each category is a `<div class="action-cat">`
- **Footer** — bottom, the colophon and disclaimers

To add a new tracker, copy one of the existing `<a class="tracker">` blocks and edit the URL, organization, title, and description.

To add an action resource, find the `<ul>` inside that category's `.resources` block and add another `<li>` following the existing pattern.

## Maintaining it

Links rot fast. Set a calendar reminder to check every 2–3 months. The Brennan Center and Protect Democracy URLs are stable; smaller orgs less so.

When the threat picture changes substantially (a new executive order, a major court ruling), update the lede paragraphs at the top.

## License

Do whatever you want with this. Fork it, rebrand it, use parts of it. It's a civic project; copying is encouraged.
