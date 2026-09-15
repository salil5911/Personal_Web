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
avoid redundant "who I am" content on two pages). The rest of the site is
`research.html`, `cv.html` (a placeholder until a real CV is ready to post), and
`contact.html`. Shared chrome (nav, footer, styles/scripts) is duplicated in each
file since there's no build step — update all files together when changing it.

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
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
