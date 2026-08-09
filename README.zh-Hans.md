<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./assets/favicon-linear-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="./assets/favicon-linear-light.svg">
    <img src="./assets/favicon-linear-light.svg" width="96" height="96" alt="One Works 图标">
  </picture>
</p>

# One Works PWA

[English](./README.md)

这个仓库发布 One Works 的独立 PWA：

https://oneworks-ai.github.io/pwa/

应用源码在 [`oneworks-ai/app`](https://github.com/oneworks-ai/app)。本仓库只保留公开 PWA 构建所需的部署 workflow 与 GitHub Pages 配置。

## 部署

`Deploy PWA` workflow 会拉取 `oneworks-ai/app`，以 `/pwa/` 作为 base 构建 `apps/client`，然后把静态产物发布到 GitHub Pages。

## 链接

- [官网](https://oneworks-ai.github.io/)
- [主仓库](https://github.com/oneworks-ai/app)
- [文档](https://oneworks-ai.github.io/docs/)
