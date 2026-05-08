# Defending the 2026 Election — Field Guide
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
