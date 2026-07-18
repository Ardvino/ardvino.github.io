# Hanna Nilsson — Portfolio

Personal portfolio website built as a single HTML file with no dependencies beyond Google Fonts.

## Structure

```
Portfolio/
├── index.html              # Entire site — markup and content
├── css/style.css           # Styles (light theme)
├── media/
│   ├── profile.jpg         # Profile photo (hero section)
│   └── background.jpg      # Hero background image
├── documentation/
│   └── resume.pdf          # Downloadable CV, linked from the hero
└── README.md
```

## Editing content

All personal content is in `index.html`. The sections follow this order:

| Section | What to edit |
|---|---|
| **Hero** | Tagline, headline, bio (`hero-eyebrow`, `h1`, `hero-bio`) |
| **About** | Background, research, teaching, location (`about-block`) |
| **Projects** | Add/edit `project-card` blocks |
| **CV** | Education, experience (`cv-entry` blocks) |
| **Skills** | `skill-item` spans inside `skills-grid` |
| **Contact** | Email and social links |

## Styling

CSS variables at the top of `<style>` control the entire look:

```css
:root {
  --accent:       #2563eb;   /* blue highlight colour */
  --bg:           #ffffff;   /* page background */
  --text:         #1f2937;   /* primary text */
  --text-muted:   #6b7280;   /* secondary text */
  --font:         'Plus Jakarta Sans', system-ui, sans-serif;
}
```

## Local preview

Open `index.html` directly in a browser, or use the **Live Server** extension in VS Code (right-click → *Open with Live Server*) for auto-refresh on save.

## Deployment

If hosted on GitHub Pages: commit changes and push to the `main` branch — the site
updates automatically within a minute.

## TODO

- [ ] Add a dedicated research page for the Alzheimer's/fMRI project (figures, methods, poster)
- [ ] Add a Publications/Presentations section once available
- [ ] Double-check `profile.jpg` framing in the circular crop
- [ ] Add a favicon
- [ ] Decide on and wire up a real deploy target (GitHub Pages / custom domain)