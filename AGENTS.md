# PWA Repository Guide

## Scope

- This repository only owns the GitHub Pages project deployment for the One Works standalone PWA at `https://oneworks-ai.github.io/pwa/`.
- Product code, package versions, and client runtime behavior live in `oneworks-ai/app`, primarily `apps/client`.
- The `main` branch should stay small: deployment workflow, repository docs, and operational notes only.
- The `gh-pages` branch is generated static output. Do not edit generated files by hand.

## Deployment

- `deploy-pwa.yml` checks out `oneworks-ai/app`, initializes the required `assets/avatar` SDK submodule before workspace install, builds `apps/client` with `__ONEWORKS_PROJECT_CLIENT_BASE__=/pwa/`, and deploys the generated static files to GitHub Pages.
- For cross-repository validation before a source PR merges, dispatch the workflow with the exact `source_sha` and `dry_run=true`; this exercises checkout, submodule initialization, install, and production build without updating `gh-pages`.
- Keep `__ONEWORKS_PROJECT_CLIENT_HOMEPAGE_PREVIEW__=1`; the homepage iframe depends on the preview runtime being present in the official PWA build.
- Keep `404.html` as a copy of `index.html` so GitHub Pages can serve React Router routes such as `/pwa/session/...` and `/pwa/rooms/...`.
