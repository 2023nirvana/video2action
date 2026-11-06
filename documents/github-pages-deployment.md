# Video2Action 科研汇报 · GitHub Pages

GitHub 账号：`2023nirvana`。唯一目标仓库：[`2023nirvana/video2action`](https://github.com/2023nirvana/video2action)，Repository name 填 `video2action`。

项目地址：<https://2023nirvana.github.io/video2action/>。使用项目仓库专用 Deploy key 更新；每次发布后核验网页内容与视频播放，并保存发布记录。

本网页为纯静态 React / Vite 站点，通过项目仓库的 GitHub Pages 提供独立项目/科研汇报主页。无需创建个人主页仓库 `2023nirvana.github.io`；网址中的 `2023nirvana.github.io` 是该账号下 Pages 的域名，`/video2action/` 是本项目入口。页面内容与视频由静态文件直接提供，无需 Sites API 或后端服务。

## 本地复现

```bash
npm ci
npm run build
npm run check
npm run preview -- --port 4173
```

浏览器打开预览服务输出的 URL。不要直接双击 `dist/index.html`，因为内容 JSON 需要由 HTTP 服务读取。

## 更新网页

1. 在 `2023nirvana` 账号下创建项目仓库 `video2action`，本次发布目标固定为 `2023nirvana/video2action`。
2. 若使用 SSH deploy key，把本次部署公钥加入该项目仓库的 Settings → Deploy keys，并勾选 `Allow write access`。Deploy key 的写入权限属于添加它的仓库，必须添加到 `video2action` 项目仓库。
3. 本地运行上述构建和检查，将完整 `dist/` 的**内容**发布到项目仓库的发布分支根目录。根目录应直接包含 `index.html`、`assets/`、`media/` 等产物，无需再创建 `video2action/` 或 `dist/` 子目录。
4. 在项目仓库 Settings → Pages 中，将 Source 设为 `Deploy from a branch`，选择实际发布分支（默认分支通常为 `main`），目录选择 `/(root)` 并保存。
5. 等待 Pages 部署成功，再核验 <https://2023nirvana.github.io/video2action/> 的页面、数据、字体与视频播放；核验前仍标记为待发布。

`vite.config.js` 中 `base: './'`，视频、字体、数据和讲稿使用相对路径。GitHub Pages 自动将项目仓库的发布根目录映射为网址中的 `/video2action/`，不需要在构建产物外额外套同名目录。

本次离线包：`科研汇报网页_20261106_2023nirvana_v5.zip`。解压后运行附带的 `serve_local.py`，通过 `http://127.0.0.1:8765/` 浏览。离线包可独立使用，不依赖线上发布状态。

所有 34 段实验视频在 `public/media/`，内容与来源在 `content/evidence.json`、`content/media_manifest.json`，源码在 `src/`。保留媒体，不将 Teacher 画面替代为 Student 输出。

## v5 阅读方式

- 第一节为当前 GVHMR 双前端完整方法图，支持放大与 SVG 下载。
- 第二节仍为六段 Overfit 独立证据。
- R37 图表以绿色标记当前模型；粗体只表示同协议内最优数值。
- 第 15 节说明推理耗时与总成本，第 16 节说明免重定向的实际范围。
- R38 仍在训练；阶段候选不能覆盖 R37 已完成的主结果。
