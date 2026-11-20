# [Your Name] — Portfolio

A one-page portfolio site for a fullstack developer, built with plain HTML and CSS
(no build step, no frameworks, no dependencies).

## Sections

- **Hero** — name, role, one-line intro, and a terminal card showing a short profile as JSON
- **Projects** — three project cards with category badge, description and tech tags
- **About** — portrait card with quick facts, plus a short bio
- **Stack** — grouped toolkit: frontend, backend, cloud & DevOps, ways of working
- **Contact** — email, LinkedIn, GitHub and résumé links

## Run it locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

## Make it yours

Everything meant to be replaced is in square brackets in `index.html`:

| Placeholder | Where |
| --- | --- |
| `[Your Name]` | page title, nav brand, hero, about card, footer |
| `[City, Country]` | hero role line, about facts |
| `[One-line intro]` | hero paragraph |
| `[3] years` | terminal card, about facts |
| `[What it is, who it's for, …]` | each of the three project cards |
| `hello@example.com` | contact section |
| `#` on LinkedIn / GitHub | contact section hrefs |

### Images

Replace the files in `assets/` (keeping the filenames, or update the `src` in the HTML):

- `assets/hero.svg` — portrait. Square-ish crops best; it is a circle on mobile.
- `assets/project-1.svg`, `project-2.svg`, `project-3.svg` — project screenshots, 16:10.

### Résumé

Drop your PDF in `assets/` and update the download link in the contact section:

```html
<a href="assets/your-cv.pdf" download>
```

## Design notes

- Dark theme, one accent colour (`--accent`), all tokens at the top of the `<style>` block
- Responsive breakpoints at 980 / 860 / 760 / 400px
- Keyboard accessible: skip link, visible focus rings, `aria-current` on the nav
- Respects `prefers-reduced-motion`

## Deploying

It is a static site, so any static host works: GitHub Pages, Netlify, Cloudflare Pages
or an S3 bucket. For GitHub Pages, go to **Settings → Pages** and set the source to
`main` / root.
