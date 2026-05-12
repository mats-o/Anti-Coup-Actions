# Defend the Next Election

A field guide for tracking federal threats to U.S. elections and taking concrete action to defend them. The live site is at **[defend2028.com](https://defend2028.com)**.

## What this is

A single-page editorial site combining:

- **Threat trackers** — links to the most credible sources monitoring federal action against U.S. elections (Brennan Center, Protect Democracy, Democracy Docket, Just Security, GovTrack)
- **Action categories** — five concrete ways to engage, ranked by impact and matched to organizations that do the work (poll work, voter protection, litigation funding, swing-state engagement, contacting representatives)

Built as a personal civic project to fill a gap: most threat-tracking organizations are 501(c)(3)s that legally can't recommend action, and most action sites don't do rigorous threat analysis. This site is a small bridge.

## How it works

The whole project is a single static HTML file (`index.html`). No build step, no framework, no dependencies. It uses:

- Plain HTML and CSS with custom typography (Fraunces and JetBrains Mono via Google Fonts)
- Two analytics scripts (Cloudflare Web Analytics and GoatCounter), both privacy-respecting and cookieless
- A small inline script for tracking outbound link clicks

Hosted on GitHub Pages with `defend2028.com` as the custom domain.

## Contributing

The link landscape changes constantly. If you find a broken link, a stale resource, or a new organization worth including:

- **Open an issue** on this repo (easiest)
- **Submit a pull request** with the change (for technical contributors)
- **Email** [contact@defend2028.com](mailto:contact@defend2028.com)

For editorial changes (adding categories, new framing, new quotes), open an issue first so we can discuss before you spend time on a PR.

## Hosting your own copy

Anyone can fork this and run their own version. The site is a single file, so:

1. Fork the repo
2. Edit `index.html` in any text editor
3. Enable GitHub Pages in your fork's settings (Settings → Pages → Source: main branch)
4. Optional: add a custom domain through your registrar

For analytics, you'll need to replace the Cloudflare and GoatCounter tokens in `index.html` with your own (they're clearly marked).

## Editing the page

The structure inside `index.html`:

- **Header** — top of file, title and intro paragraphs
- **Trackers** — `<section id="track">`, each tracker is an `<a class="tracker">`
- **Actions** — `<section id="act">`, each category is a `<div class="action-cat">`
- **Footer** — bottom, the colophon and disclaimers

To add a new tracker, copy one of the existing `<a class="tracker">` blocks and edit the URL, organization, title, and description.

To add an action resource, find the `<ul>` inside that category's `.resources` block and add another `<li>` following the existing pattern.

## Maintenance

Links rot fast. Aim to check every 2–3 months. The Brennan Center and Protect Democracy URLs are stable; smaller organizations less so. When the threat picture shifts substantially (a major executive order, a significant court ruling), update the lede paragraphs and the "Last updated" date in the footer.

## License

MIT License. Use, modify, and redistribute freely. Attribution appreciated but not required.

## Disclaimer

This is a personal civic project, not affiliated with any organization linked from the site. All trackers and groups linked are credibly nonpartisan or transparent about their orientation. Inclusion is editorial judgment, not endorsement.

