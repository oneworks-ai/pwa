<p align="center">
  <img src="https://oneworks-ai.github.io/favicon-metal-light-transparent.svg" width="96" height="96" alt="One Works icon">
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
