# Plango 官网（plango.one）

这是 **[liusqu/plango-site](https://github.com/liusqu/plango-site)** 的部署仓库，
线上站点通过 GitHub Pages + custom domain `plango.one` 托管。

主页设计源：`Plango_iOS/docs/design/homepage-v2/index.html`。

改动流程：在私有仓库完成设计与浏览器验收，再同步到本部署仓库：

```bash
# 同步 homepage-v2/index.html、该文件实际引用的 assets、site/privacy.html
# 与 site/terms.html。不要整包复制 homepage-v2/assets，里面包含 4K 评审母片。
cd ../plango-site && git add -A && git commit -m "sync from Plango_iOS site/" && git push
```

背景与台账见 `docs/prd/growth/growth-review-2026-07-12.md`（G-3/G-4）。
DNS：plango.one 在 Squarespace 注册，需按台账 §五 指向 GitHub Pages。
