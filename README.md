<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./assets/favicon-linear-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="./assets/favicon-linear-light.svg">
    <img src="./assets/favicon-linear-light.svg" width="96" height="96" alt="One Works icon">
  </picture>
</p>

# One Works PWA

[简体中文](./README.zh-Hans.md)

This repository publishes the standalone One Works PWA at:

https://oneworks-ai.github.io/pwa/

The application source lives in [`oneworks-ai/app`](https://github.com/oneworks-ai/app). This repository only contains the deployment workflow and GitHub Pages configuration for the public PWA build.

## Deployment

The `Deploy PWA` workflow checks out `oneworks-ai/app`, builds `apps/client` with the `/pwa/` base path, and deploys the generated static site to GitHub Pages.

## Links

- [Homepage](https://oneworks-ai.github.io/)
- [App repository](https://github.com/oneworks-ai/app)
- [Documentation](https://oneworks-ai.github.io/docs/)
