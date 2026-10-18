# 知微的个人网站 / Zhiwei's personal website

纯静态 HTML + CSS + JavaScript 制作，无需安装依赖、无需构建，可以直接部署到 GitHub Pages。
A dependency-free bilingual static site ready for GitHub Pages.

## 本地预览 / Local preview

直接双击 `index.html`，或者运行 `python -m http.server 8000` 后打开 http://localhost:8000。
Open `index.html` directly, or serve the folder locally with `python -m http.server 8000`.

## 部署到 GitHub Pages / Deploy

1. 登录 GitHub，新建 **public** 仓库，仓库名设为 `<你的GitHub用户名>.github.io`（例如 `octocat.github.io`）。
2. 上传此文件夹里的 **所有文件** 到仓库的根目录（包括 `index.html`、`styles.css`、`script.js`、`favicon.svg`）。不要额外套一个 `zhiwei-site` 文件夹。
3. 进入仓库 **Settings → Pages → Build and deployment**，选择 **Deploy from a branch**、`main`、`/(root)`，然后保存。
4. 部署完成后访问 `https://<你的GitHub用户名>.github.io/`。GitHub Pages 可能需要几分钟刷新。

Or use an existing repository and publish it to `https://<username>.github.io/<repo>/` using the same Pages settings.

## 定制 / Customize

- 打开 `script.js`，将 `const GITHUB_USERNAME = "";` 改成你的 GitHub 用户名。
- 打开 `index.html` 修改文字、项目、标题。双语内容应同时编辑 `script.js` 内 `copy.zh` 和 `copy.en`。
- 在 `styles.css` 的 `:root` 部分修改配色。
- 摄影板块当前是 CSS 插画占位，替换真实照片可在 `index.html` 相应位置加入 `<img src="your-photo.jpg" alt="...">` 并自行调整 CSS。
- 建议在公开发布前检查所有文字与项目状态，不要放私人联系方式、地址或其他不想公开的信息。

## Features

- 中英双语切换 / Chinese-English toggle
- 深色模式 / Dark mode
- 手机适配 / Responsive layout
- 阅读进度条 / Scroll progress
- 无框架、无构建 / No frameworks or build step

字体在线加载 Google Fonts；若无法访问，会自动使用本地后备字体。页面本身无需联网 API。
