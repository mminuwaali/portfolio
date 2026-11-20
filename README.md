# Muhammad Muhammad Inuwa — Portfolio

A one-page portfolio for a fullstack software engineer, built with plain HTML and CSS
(no build step, no frameworks, no dependencies).

Live: <https://mimi-coding.github.io/portfolio/>

## Sections

- **Hero** — name, role, positioning line, and a terminal card showing a short profile as JSON
- **Projects** — BuildStock, Noma inventory platform, and VueBoard
- **About** — portrait, quick facts, and a short bio
- **Stack** — grouped toolkit: frontend, backend, data, cloud & DevOps, ways of working
- **Experience** — Coave (Frontend Team Lead), Kwari E-Market, and earlier work
- **Contact** — email, LinkedIn, GitHub and résumé

## Content sources

Everything on the page was taken from the GitHub profile README at
<https://github.com/mminuwaali/mminuwaali>, plus the public repo metadata
(homepages, descriptions) and the avatar from <https://github.com/mminuwaali>.

## Run it locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

## Keeping it current

| What | Where |
| --- | --- |
| Bio, facts, experience | `index.html` — `#about`, `#experience` |
| Projects | `index.html` — `#work` (title, description, tags, link) |
| Stack tags | `index.html` — `#stack` |
| Email / LinkedIn / GitHub | `index.html` — `#contact` |
| Résumé PDF | put the file in `assets/` and update the download link |
| Portrait | `assets/avatar.jpg` (square, 460×460) |

## Design notes

- Dark theme, one accent colour (`--accent`), all tokens at the top of the `<style>` block
- Responsive breakpoints at 980 / 860 / 760 / 400px
- Keyboard accessible: skip link, visible focus rings, `aria-current` on the nav
- Respects `prefers-reduced-motion`

## Deploying

Static site — GitHub Pages serves `main` / root. `.nojekyll` keeps files served as-is.
