# Dennis Schuster - Interactive Resume

A bilingual, privacy-conscious static resume for GitHub Pages.

## Features

- English and German content with `?lang=en` / `?lang=de` deep links
- Responsive single-page layout
- Expandable professional timeline with concise/expanded views
- Light and dark themes
- Two-page, A4-ready PDF summary through the browser print dialog
- Keyboard-friendly controls, semantic structure, focus styles, and reduced-motion support
- No framework, build step, cookies, analytics, tracking, external fonts, or network dependencies
- No email address, phone number, street address, birth information, manager names, internal ratings, or source documents

## Publish on GitHub Pages

1. Create a new GitHub repository.
2. Upload the contents of this folder to the repository root:
   - `index.html`
   - `.nojekyll`
   - `assets/portrait.jpg`
3. Commit the files.
4. Open **Settings > Pages** in the repository.
5. Under **Build and deployment**, select **Deploy from a branch**.
6. Select the `main` branch and `/ (root)`, then save.
7. GitHub will show the published site URL after deployment.

## PDF summary

Choose **PDF summary** / **PDF-Kurzprofil**. The browser print dialog opens with a compact two-page A4 layout in the currently selected language.

Recommended settings:

- Destination: **Save as PDF**
- Paper size: **A4**
- Scale: **100%**
- Margins: **Default** or **None** (the page stylesheet already sets print margins)
- Background graphics: **Enabled** for the intended styling
- Headers and footers: **Disabled**

## Local preview

You can open `index.html` directly. For a local web server, run:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000/`.

## Customize

Most content is directly in `index.html`. Search for `data-lang="en"` and `data-lang="de"` to edit language-specific text. The design tokens are CSS variables near the top of the file.

The portrait is stored locally at `assets/portrait.jpg`; its metadata was removed for privacy.
