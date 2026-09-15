# Salil Verma — Personal Website

A fast, dependency-free personal/academic site for Salil Verma, PhD student at the
School of Computer and Cyber Sciences, Augusta University. Research focus: human
sensing, IoT privacy, and human-computer interaction.

Built with plain HTML/CSS/JS (no build step) in a clean, light, Jekyll/al-folio-style
academic template: circular profile photo, serif name, a single accent color, flat
bordered cards, and minimal scroll-reveal — no particle backgrounds, gradients, or
glow effects.

## Pages

`index.html` is the homepage and doubles as the About page (intro + bio, merged to
avoid redundant "who I am" content on two pages). The rest of the site lives one
folder deep as `research/index.html`, `cv/index.html` (a placeholder until a real
CV is ready to post), and `contact/index.html` — GitHub Pages serves a folder's
`index.html` at the folder's URL, so the site links as clean paths
(`/research/`, `/cv/`, `/contact/`) with no `.html` or filename showing in the
address bar. Shared chrome (nav, footer, styles/scripts) is duplicated in each
file since there's no build step — update all files together when changing it,
and use root-relative links (e.g. `/Personal_Web/research/`) everywhere since
pages live at different folder depths.

## Local preview

```bash
cd .. && python3 -m http.server 8000
# open http://localhost:8000/Personal_Web/
# (served from the parent folder so the root-relative /Personal_Web/... links
# resolve the same way they do on GitHub Pages)
```

## Deploying (GitHub Pages)

This repo includes `.github/workflows/deploy.yml`, which deploys automatically on
every push to `main` using GitHub Actions.

One-time setup: in the repo's **Settings → Pages**, set **Source** to
**GitHub Actions**. After that, every push to `main` publishes the live site.

## Things to personalize

- `salverma@augusta.edu` — the public contact email (Contact page and mailto
  links across all pages). Swap it if you'd rather show a different address.
- `https://github.com/salil5911` — update if this isn't your GitHub handle, or add
  LinkedIn/X/ORCID links next to it in the hero and contact sections.
- `assets/img/og-image.png` — regenerate if you change name/title (script not
  included in repo; ask to have it regenerated with new details).
