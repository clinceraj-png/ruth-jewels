# ruth-jewels

A handcrafted South Indian jewellery showcase built as a static site. This repository includes the live landing page at `index.html` and a small local Python helper for scanning product images, generating metadata, and previewing the current collection.

## Quick start

- Open `index.html` in your browser to view the site.
- Use `python3 agent.py list` to list discovered product images.
- Use `python3 agent.py generate` to regenerate `products.json` and `product-catalog.html`.

## GitHub Pages deployment

The site is configured to publish as a static GitHub Pages site from the `main` branch.

What is already set up:
- A GitHub Actions workflow at `.github/workflows/deploy-pages.yml`
- A `.nojekyll` file so Pages serves the site without Jekyll processing

After pushing these changes to GitHub, enable GitHub Pages in the repository settings:
1. Go to Settings → Pages
2. Under "Build and deployment", choose "GitHub Actions"
3. Save the setting and wait for the workflow run to finish

Once published, the site will be available at:
- `https://<your-username>.github.io/ruth-jewels/`

## Notes

- Product asset files are stored under `images/`.
- The helper script is compatible with Python 3.8 and newer.
