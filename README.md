# Arvin Björkgren — Portfolio

Personal portfolio website built as a single HTML file with no dependencies beyond Google Fonts.

## Structure

```
Portfolio/
├── index.html       # Entire site — markup, styles, and content
├── profile.png      # Profile photo (hero section)
├── background.jpg   # Hero background image
└── README.md
```

## Editing content

All personal content is in `index.html`. The sections follow this order:

| Section | What to edit |
|---|---|
| **Hero** | Tagline, quote, bio (`hero-eyebrow`, `h1`, `hero-attr`, `hero-bio`) |
| **About** | Background, research, interests, location (`about-block`) |
| **Projects** | Add/edit `project-card` blocks |
| **CV** | Education, research, clinical experience (`cv-entry` blocks) |
| **Skills** | `skill-item` spans inside `skills-grid` |
| **Contact** | Email and social links |

## Styling

CSS variables at the top of `<style>` control the entire look:

```css
:root {
  --accent:       #60a5fa;   /* blue highlight colour */
  --bg:           #0d1117;   /* page background */
  --text:         #e6edf3;   /* primary text */
  --text-muted:   #8b949e;   /* secondary text */
  --font:         'Plus Jakarta Sans', system-ui, sans-serif;
}
```

## Local preview

Open `index.html` directly in a browser, or use the **Live Server** extension in VS Code (right-click → *Open with Live Server*) for auto-refresh on save.

## Deployment

Hosted on GitHub Pages at `https://ardvino.github.io`.

To update: commit changes and push to the `main` branch — the site updates automatically within a minute.