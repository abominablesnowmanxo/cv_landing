# Andrey Kuznetsov CV Landing Page

Static one-screen CV landing page for GitHub Pages.

Live site:
https://abominablesnowmanxo.github.io/cv_landing/

## Structure

- `index.html` - page content, section markup, links, and keyboard navigation script.
- `static/styles.css` - all layout, typography, colors, and responsive styling.
- `static/images/photo.JPG` - profile photo.
- `static/images/certificates/` - certificate preview images.
- `assets/andrey-kuznetsov-cv-2026.pdf` - bundled CV copy kept in the repo, though the main button currently links to Google Drive.

## Local Preview

This site has no build step and no framework. You can open `index.html` directly in a browser.

For a local server preview:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Updating Content

- Main profile text and social links are in `index.html`.
- Skills are in the `panel-skills` section.
- Experience entries are in the `panel-experience` section.
- Certifications are in the `panel-certificates` section.
- Colors, spacing, font sizing, and panel layout are in `static/styles.css`.

## Controls

- Header buttons open the related section.
- `ArrowLeft` / `ArrowRight` cycles through the main page and sections.
- In Experience and Certifications, `ArrowUp` / `ArrowDown` changes the selected item.
- `Escape` closes the active section.

## Deployment

The project is GitHub Pages-friendly as plain static files. Push changes to the configured Pages branch, and GitHub Pages will serve the updated `index.html`, `static/`, and `assets/` files.
