# Bigtail Landing Page

Static deployment of the Switch landing page template, prepared for GitHub Pages hosting.

## Deploying to GitHub Pages
1. Push the contents of this repository to GitHub.
2. In **Settings → Pages**, choose **Deploy from a branch** with **Branch: `main`** and **Folder: `/ (root)`**.
3. After Pages finishes building, your site will be available at `https://<username>.github.io/<repo>/` (replace `<repo>` with the repository name if it changes).

## Local development
* Requires Node.js 14 (use [NVM](https://github.com/nvm-sh/nvm) to manage versions).
* Install dependencies: `npm install`.
* Start live development server with rebuilds and browser reloads: `npm run watch`.
* Produce a fresh production bundle: `npm run build` (outputs to `dist/`).
* Clean generated assets: `npm run clean`.

## Project structure
* `index.html` – main entry point that references assets in `dist/`.
* `dist/` – compiled CSS/JS/images ready to serve on GitHub Pages.
* `src/` – SCSS, JS, and image sources used for rebuilding the landing page.
* `package.json` – scripts and dev dependencies for local development.
