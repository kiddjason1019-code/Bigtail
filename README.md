# Bigtail Landing Page

This repository hosts the Switch landing page extracted from the included `switch.zip` archive and prepared for GitHub Pages deployment.

## Project structure
- `switch/`: Static site sources and compiled assets (`dist/`) used by the landing page. A `.nojekyll` file is included so Pages serves everything as-is.
- `switch.zip`: Original archive provided for reference.
- `.github/workflows/deploy-pages.yml`: GitHub Actions workflow that publishes the `switch` directory to GitHub Pages.

## Preview locally
1. From the repository root, serve the `switch` folder (for example with Python):
   ```bash
   python -m http.server 8000 --directory switch
   ```
2. Open http://localhost:8000 in your browser to view the page.

## Deployment
GitHub Pages deployment is automated via GitHub Actions:
- Every push to the `work` branch uploads the contents of `switch/` and deploys them to the `github-pages` environment.
- To activate the site the first time, open the repository settings and set **Pages** to use the **GitHub Actions** source if it is not already enabled.

Once configured, the published site will be available at your repository's GitHub Pages URL.
