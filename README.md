# Mohit Ahirwar — Portfolio

Personal portfolio site. **Live:** [ahirwarmohit.github.io](https://ahirwarmohit.github.io)

Vanilla HTML, CSS and a little JavaScript. No build step, no dependencies. Edit a file, commit, done.

## Structure

```
/
├── index.html                          Home
├── cv.html                             CV
├── bcv.html                            CV, banking and consulting version
├── articles.html                       Writing index
├── article-beyond-the-prompt.html      Article
├── yono-case-study.html                SBI YONO 2.0, insurance vertical
├── mdes-thesis.html                    Cozy Nights, M.Des thesis
├── global-adaptive-design-system.html  Global Adaptive Design System
└── assets/
    ├── styles.css                      Shared tokens and components
    ├── favicon.svg · favicon.ico
    ├── og-image.png
    ├── profile/                        Portrait imagery
    ├── yono/                           Case study screens
    └── work/                           Homepage tile loops and posters
```

## Design system

Tokens live in one place: `assets/styles.css`. Do not redefine them per page.

| | |
|---|---|
| Display | Fraunces 300, with Instrument Serif italic for emphasis |
| Body | IBM Plex Sans |
| Labels, data | IBM Plex Mono, uppercase, tracked |
| Accent | `--blue: #1a4ed8` |
| Section tints | `--sand: #f5efe4`, `--sage: #ecf0eb` |
| Radius | 3px |

Light mode only. No dark theme.

## Adding a page

1. Copy the `<head>` from `index.html`, including the `assets/styles.css` link.
2. Reuse `.nav` and `.foot` markup as-is.
3. Put only page-specific CSS in an inline `<style>` block.

## Homepage tile loops

Each work card and the OCS tile take a silent looping MP4 with a poster fallback. Loops play only while in the viewport and are skipped entirely under `prefers-reduced-motion`.

Specification: 6–10 seconds, silent, H.264, under 2 MB, cropped tight on a single interaction rather than a whole flow.

```
assets/work/yono-loop.mp4         + yono-poster.jpg
assets/work/cozy-loop.mp4         + cozy-poster.jpg
assets/work/gads-loop.mp4         + gads-poster.jpg
assets/work/ocs-logo-reveal.mp4   + ocs-poster.jpg
assets/work/speaking.jpg
assets/work/sketchbook.jpg
assets/profile/portrait.jpg
```

Until a file exists, the card shows a neutral placeholder rather than a broken frame.

## Accessibility

Skip link, visible keyboard focus, reduced-motion honoured throughout, custom cursor disabled on touch and for reduced-motion users.

## Contact

**Mohit Ahirwar** · [mohitahirwar7@gmail.com](mailto:mohitahirwar7@gmail.com) · [LinkedIn](https://www.linkedin.com/in/mohit-ahirwar/)
