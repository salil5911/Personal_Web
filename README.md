# Salil Verma — Personal Website

A fast, dependency-free personal/academic site for Salil Verma, PhD student at the
School of Computer and Cyber Sciences, Augusta University. Research focus: human
sensing, IoT privacy, and human-computer interaction.

Built with plain HTML/CSS/JS (no build step) — a canvas particle network background,
scroll-reveal animations, a typewriter hero, and a terminal-style "about" card.

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

- `salilverma514@gmail.com` — swap for whichever email you want public (Contact
  section and mailto links in `index.html`).
- `https://github.com/salil5911` — update if this isn't your GitHub handle, or add
  LinkedIn/X/ORCID links next to it in the hero and contact sections.
- `assets/img/og-image.png` — regenerate if you change name/title (script not
  included in repo; ask to have it regenerated with new details).
- Consider adding a headshot/photo to the hero or about section.
