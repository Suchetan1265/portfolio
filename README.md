# Suchetan Mukherjee — Portfolio

A single-page personal portfolio site. Static HTML/CSS/JS — no build step, no
dependencies. Open it anywhere.

**Live page:** publish `index.html` to any static host (see *Deploy* below).

## What's inside

```
portfolio/
├── index.html                         # the whole site (self-contained)
├── assets/
│   └── Suchetan_Mukherjee_Resume.pdf   # linked from the Résumé buttons
└── README.md
```

Sections: hero (animated event-pipeline canvas), highlights, what I build,
experience, projects, tech stack, achievements & publications, education, and
contact. Dark/light theme toggle, responsive down to phone width, respects
`prefers-reduced-motion`.

## View locally

Just open `index.html` in a browser (double-click), or serve the folder:

```bash
python -m http.server 8000
# then open http://localhost:8000
```

Serving (rather than file://) makes the Résumé PDF link resolve cleanly.

## Customize

Everything is plain text in `index.html`:

- **Contact** — email, phone, LinkedIn and GitHub are in the hero and the
  `#contact` section.
- **Experience / Projects / Education** — each is a labelled block of markup;
  edit the text in place.
- **Résumé** — replace `assets/Suchetan_Mukherjee_Resume.pdf` to update the
  downloadable PDF.
- **Colours & fonts** — the `:root` block at the top of the `<style>` holds every
  design token (cobalt accent, slate neutrals, Sora / Hanken Grotesk / JetBrains
  Mono).

## Deploy

**GitHub Pages**

```bash
# after pushing this folder to a GitHub repo:
# Settings → Pages → Branch: main, folder: / (root) → Save
# site goes live at https://<username>.github.io/<repo>/
```

**Netlify / Vercel / Cloudflare Pages** — drag the folder in, or point it at the
repo. No build command; publish directory is the folder root.

---

Built with code, not templates.
