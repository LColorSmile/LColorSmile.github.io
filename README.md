# 浅浅笑微的博客

博客地址：[https://lcolorsmile.github.io/](https://lcolorsmile.github.io/)

此仓库使用 Hexo 7.3.0 和 Butterfly 5.5.4 构建。站点名称、头像、文章和标签从原有 Gmeek 博客保留。原 Gmeek 配置、生成页面及工作流存放在仓库中，便于回退；旧工作流位于 `.github/legacy/Gmeek.yml`，不会继续自动部署。

## 写作与预览

文章放在 `source/_posts/`，使用 Markdown 和 YAML front matter。文章的 `categories` 与 `tags` 决定分类和标签页面。

```bash
npm ci
npm run build
npm run preview
```

本地预览地址是 `http://localhost:4000/`。修改首页和侧栏文字、头像、配色时，编辑 `_config.yml` 与 `_config.butterfly.yml`；首页背景位于 `source/img/hero-soft.svg`。

## 部署

合并到 `main` 后，`Build and deploy Hexo` 工作流构建 `public/` 并通过 GitHub Pages 部署。仓库的 **Settings → Pages → Build and deployment → Source** 需设为 **GitHub Actions**。Pull Request 只构建检查，不部署。

原 Gmeek 文章仍保留在 [GitHub Issues](https://github.com/LColorSmile/LColorSmile.github.io/issues) 中；迁移后的文章保留原有 `post/ce-shi.html` 地址。
