# 封面工坊 · Cover Studio

一个浏览器里就能用的封面 / Banner 生成器。专为文章题图、社交媒体封面、视频缩略图设计。

## 在线使用

[点这里打开](https://shirleyxiaolulu.github.io/cover-studio/)

## 功能

- **图片拼图** — 1 / 2 / 3 张横排拼接，无间隔；每张独立缩放 + 位置调整（支持拖拽）
- **标题 + 副标题** — 画布上直接点击编辑；字体 / 字重 / 字号 / 颜色 / 透明度 / 对齐都可调
- **两种排版** — 居中多行 / 左下单行
- **样式预设** — 6 个内置预设，可保存自己的，可拖动排序，可导出/导入 JSON 备份
- **模板** — 7 个内置模板（拼图数 + 样式 + 间距 + 尺寸的完整骨架），可"另存为模板"
- **多画布** — 一次做多个封面，画布列表底部切换 / 复制 / 删除
- **批量导出** — 一键导出所有画布，支持选择目标文件夹（Chrome / Edge）
- **导出** — PNG 格式，2× 超采样保证文字锐利；可选导出尺寸（默认 1200×350，支持 1:1、16:9、9:16 等）
- **撤销/重做** — ⌘Z / ⌘⇧Z；所有操作都进历史栈
- **自动保存** — 所有数据存在浏览器 localStorage，刷新不丢；额外提供导出 JSON 备份

## 技术

- 纯前端 · 单 HTML 文件 · 零构建步骤
- React 18（CDN）+ Babel Standalone 实时编译 JSX
- Canvas API 渲染导出（2× SSAA）
- File System Access API 用于选择导出位置（仅 Chromium）
- 字体：Noto Sans SC / Noto Serif SC / Bricolage Grotesque（Google Fonts）

## 浏览器支持

- **推荐**：Chrome 86+ / Edge 86+ / Arc — 完整功能，含文件夹选择
- **可用**：Safari 14+ / Firefox 90+ — 导出会落到默认下载目录
- 移动端未优化，建议桌面使用

## 数据存储

所有数据（画布、上传图、样式预设、模板）都在你的浏览器 localStorage 里，**不会上传到任何服务器**。每个用户在自己浏览器里的数据互相隔离。建议偶尔用"导出预设 JSON"做备份。

## 部署

最简单的方式：[GitHub Pages](https://pages.github.com/)

1. 把这个仓库 fork 或者把 `index.html` 上传到你自己的仓库
2. Settings → Pages → Source 选 `main` 分支 → Save
3. 一分钟后访问 `https://你的用户名.github.io/仓库名/`

或者任何能托管静态文件的服务都行（Vercel / Netlify / Cloudflare Pages / 自己服务器）。

## License

MIT
