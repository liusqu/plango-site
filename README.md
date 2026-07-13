# Plango 官网（plango.one）

**这里是设计源，不是部署点。** Plango_iOS 是私有仓库（免费 plan 开不了 GitHub Pages），
线上站点由 public 仓库 **[liusqu/plango-site](https://github.com/liusqu/plango-site)** 托管
（GitHub Pages + custom domain plango.one）。

改动流程：在本目录改 → 同步到 plango-site：

```bash
# 从 monorepo 根目录
rsync -av --delete --exclude .git site/ ../plango-site/
cd ../plango-site && git add -A && git commit -m "sync from Plango_iOS site/" && git push
```

背景与台账见 `docs/prd/growth/growth-review-2026-07-12.md`（G-3/G-4）。
DNS：plango.one 在 Squarespace 注册，需按台账 §五 指向 GitHub Pages。
