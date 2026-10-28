# 数独扫雷 · Sudoku Minesweeper

在线免费小游戏：标准 9×9 数独 + 扫雷式隐藏地雷。四种模式：经典（0 雷）、简单（5 雷）、困难（10 雷）、17 数（12 雷）。

## 本地运行

```bash
python -m http.server 8080
# 打开 http://localhost:8080/
```

纯静态站点，没有构建步骤，没有后端依赖。

## 文件结构

- `index.html` — 游戏 + 首页内容
- `how-to-play.html` — 完整规则
- `strategies.html` — 数独技巧
- `about.html` / `privacy.html` — 关于与隐私政策
- `feedback.html` — 双语反馈页（mailto / Gmail / Issues）
- `style.css` / `sudoku.js` — 样式与游戏逻辑
- `assets/` — favicon 与 OG 封面
- `sitemap.xml` / `robots.txt` / `ads.txt`

## 部署

推送到 GitHub，仓库 Settings → Pages → Deploy from branch `main` / root。站点地址：https://yangfanwudi.github.io/sudoku-site/

## 广告位

首页与文章页预留了 `.ad-slot` 容器，审核通过前为空、不显示。AdSense 脚本注释在 `index.html` 等页面的 `<head>` 中。
