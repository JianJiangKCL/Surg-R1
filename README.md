# Surg-R1 — Project Homepage

**Live site:** <https://jianjiangkcl.github.io/Surg-R1/>

## Quick Reference

| Item | Location / Value |
|------|-----------------|
| Live URL | `https://jianjiangkcl.github.io/Surg-R1/` |
| GitHub repo | `https://github.com/JianJiangKCL/Surg-R1` |
| Deploy source | `main` branch / root (`/`) |

## Editable Content

All content lives in `index.html`. Below is a quick guide to what you can change and where to find it.

### Hero Section (line ~30)

- **Badge text** — `<span class="badge">...</span>` (currently "Surgical AI Research")
- **Title** — `<h1>` tag
- **Subtitle** — `<p class="hero-sub">`
- **Key stats** — four `.stat` blocks (Parameters / CoT Pairs / Datasets / Arena Score)
- **Buttons** — GitHub link URL in `.hero-actions`

### Demo Video (line ~67)

- Video file: `assets/videos/surgr1-demo-web.mp4`
- To replace the video, put a new `.mp4` in the same path (keep the filename, or update the `<source>` tag)

### Abstract (line ~81)

- Three `<p>` paragraphs inside `.abstract-card`
- Update text directly; use `<strong>` for bold

### Experimental Results (line ~93)

- **Figure 1** image: `assets/images/figure2.png` (training data + benchmarks)
- **Figure 2** image: `assets/images/figure1.png` (overview + radar charts)
- To replace figures, overwrite the PNG files or update `src` in the `<img>` tags
- Captions are in `<figcaption>` below each image

### Method Overview (line ~115)

- Four `.method-card` blocks (Level 1 / Level 2 / Level 3 / Pipeline)
- Each has an icon (`<i class="fa-solid fa-...">`) , heading `<h3>`, and description `<p>`

### Authors (line ~144)

- Author name pills in `.author-list`
- CSS classes: `equal` = equal contribution highlight, `corresponding` = corresponding author highlight
- Superscript affiliations: `<sup>1,†</sup>` etc.
- Affiliation list in `<ol class="affil-list">`

### Contact (line ~192)

- Corresponding author name and email in `.contact-card`

### Footer (line ~201)

- Copyright text, GitHub link, email link

## Styling

- All styles are in `styles.css`
- Uses [Inter](https://fonts.google.com/specimen/Inter) font (Google Fonts) and [Font Awesome 6](https://fontawesome.com/) icons
- Color scheme defined in `:root` CSS variables at the top of `styles.css`

## Local Preview

```bash
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Deployment

Push to `main` and GitHub Pages auto-builds within ~30 seconds.

```bash
git add .
git commit -m "update content"
git push origin main
```
