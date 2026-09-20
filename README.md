# 陈莅谋 · Portfolio

面向求职展示的个人网站，重点介绍正在推进的双侧不确定性算电协同研究。内容与 [当前研究仓库](https://github.com/Brolem/compute_energy_bilateral_uncertainty) 的 README 对齐；尚未完成的优化器和样本外实验不展示为正式成果。网站包含 PDF 简历和用户提供的 Big Five 测评嵌入页。

## 本地运行

需要 Node.js 24 或兼容版本。

```bash
npm ci
npm run dev
```

构建静态页面：`npm run build`，输出至 `dist/`。

## GitHub Pages

将源码推送到 `Brolem/Brolem.github.io` 仓库的 `main` 分支，在仓库 **Settings → Pages → Build and deployment → Source** 选择 **GitHub Actions**。项目内的 `.github/workflows/deploy.yml` 会在推送时构建和部署。网站地址为 `https://brolem.github.io/`。

首页：`src/pages/index.astro`；研究案例：`src/pages/projects/bilateral-uncertainty.astro`；共用样式：`src/styles/global.css`。研究进度变化时，应同步更新案例页，尤其是“当前关键发现”和“待完成的验证”。
