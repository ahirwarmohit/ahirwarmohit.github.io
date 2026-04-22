# Mohit Ahirwar — Portfolio

Personal portfolio website for **Mohit Ahirwar**, Product Designer & UX Lead. M.Des, IIT Delhi.

**Live URL (after deployment):** `https://ahirwarmohit.github.io`

---

## File Structure

```
/
├── index.html                          ← Landing page / home
├── cv.html                             ← Curriculum Vitae
├── yono-case-study.html                ← Case Study 01: YONO 2.0 Insurance
├── global-adaptive-design-system.html  ← Case Study 02: Design Systems [fill in]
├── mdes-thesis.html                    ← Case Study 03: M.Des Thesis [fill in]
├── assets/
│   ├── favicon.svg                     ← SVG favicon (MA monogram, blue)
│   ├── favicon.ico                     ← ICO fallback
│   └── og-image.png                    ← Open Graph share image [replace]
└── README.md                           ← This file
```

---

## How to Deploy to GitHub Pages

1. Create a repository named `ahirwarmohit.github.io` on GitHub
2. Upload all files (maintaining the folder structure above)
3. Go to **Settings → Pages → Source** → select `main` branch, `/ (root)`
4. Your site will be live at `https://ahirwarmohit.github.io` within minutes

**Alternative:** Drag-and-drop the entire folder to [Netlify Drop](https://app.netlify.com/drop) or [Vercel](https://vercel.com) for instant deployment.

---

## How to Update Content

All pages use **vanilla HTML + CSS + minimal JavaScript**. No build step required.

- Edit text directly in any `.html` file with a text editor (VSCode recommended)
- All design tokens (colours, fonts) are in the `:root` CSS block at the top of each file
- Do not change font families or colour variables — they define the visual identity

### Adding Your Photo

In `cv.html`, find the `h-photo` div and replace the placeholder with:
```html
<img src="assets/photo-mohit.jpg" alt="Mohit Ahirwar">
```
Upload `photo-mohit.jpg` to the `assets/` folder. Recommended: square crop, min 600×600px.

### Updating the OG Image

Replace `assets/og-image.png` with a 1200×630px PNG. Recommended: dark background (`#141210`) with your name in white text.

---

## Placeholder Index

The following `[PLACEHOLDER]` markers need to be filled before the site is complete. Search each file for `[PLACEHOLDER]` to locate them.

### `global-adaptive-design-system.html`
| Location | Placeholder |
|---|---|
| Cover `<h1>` | Update thesis/project title if different from "Global Adaptive Design System" |
| Cover `meta-value` (col 5) | Project output type |
| Section 01 — Context | Research context, motivating problem, sponsor/institution |
| Section 01 — Callout | Core thesis question |
| Section 02 — Challenge | Specific challenge description, fieldwork, literature review |
| Section 03 — Approach | Research methodology, key findings |
| Section 03 — highlight-box | Key insight or pivot moment |
| Section 04 — System | Architecture description, framework details |
| Principle Cards 04–06 | Additional design principles |
| Section 04 — placeholder-notice | Replace with actual diagrams/screenshots |
| Section 04 — pull-quote | Quote from advisor or thesis |
| Section 05 — Outcomes | Actual project outcomes 01, 02, 03 |
| Section 05 — para 2 | Other professional connections |

### `mdes-thesis.html`
| Location | Placeholder |
|---|---|
| Cover `<h1>` | Actual thesis title |
| Cover `meta-value` (advisor) | Thesis advisor's name |
| Cover `cover-sub` | Thesis abstract (1–2 sentences) |
| Section 01 — Context | Research domain and motivation |
| Section 01 — gap | Knowledge gap this thesis fills |
| Section 01 — Callout | Core research question |
| Section 02 — Research | Methodology description |
| Process steps 01–06 | Actual research phases |
| Section 02 — highlight-box | Key research insight |
| Section 03 — Design | Design output description |
| Section 03 — placeholder-notice | Replace with actual visuals |
| Section 03 — pull-quote | Advisor quote or design principle |
| Section 04 — Outcomes | Actual thesis outcomes 01, 02 |
| Section 05 — Reflection | Personal reflection (first para) |
| Section 05 — Callout | Connection to professional work |

---

## Technical Notes

- **No frameworks or build tools.** Pure HTML/CSS/JS — edit and open in any browser.
- **Google Fonts** are loaded via CDN (Fraunces + IBM Plex Sans + IBM Plex Mono). Internet connection required to load fonts.
- **Page transitions** work by fading the body on internal `.html` link clicks. This is CSS animation only.
- **Scroll reveal** uses `IntersectionObserver` — no polyfill needed for modern browsers.
- **Print stylesheet** is embedded in `cv.html` only (the other pages don't need it).
- **Hamburger menu** activates at ≤1000px viewport width (or ≤900px on the YONO case study page).

---

## Contact

**Mohit Ahirwar** — mohitahirwar7@gmail.com  
LinkedIn: [linkedin.com/in/mohit-ahirwar](https://www.linkedin.com/in/mohit-ahirwar/)
