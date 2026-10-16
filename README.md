# Chen LM · Portfolio

面向求职展示的个人网站，展示 Chen LM 的研究、学习进展与工作方式。当前研究主线为双侧不确定性算电协同，实习关注能源数字化、算力资源与成本分析、优化决策相关方向。网站包含公开版 PDF 简历和用户提供的 Big Five 测评嵌入页。

## 内容维护（2026-10-16）

首页定位为简洁个人主页，以自我介绍、近期学习、项目简述和做事方式为主。技术协议、实验数字和结论边界放在项目案例页；不把首页恢复为研究报告或技术能力清单。Big Five 保留在可展开区域。

- 研究事实以现役仓库的最新 README、科学协议及实验台账为依据；当前 V2 四组对照各完成 21 天 Validation，V2 OOS 尚未运行。历史协议的 OOS 不替代当前协议。
- 本窗口联合场景未显示成本优势；保留当日真实值已知、未来日前代理、独立积场景与自由末储能状态等结论边界，不宣称在线或样本外优势。
- 当前重点是有日期的项目状态，后续依据仓库状态说明更新。已放弃的两个旧算电项目不列为精选成果，不沿用其收益数字。
- 个人仍在项目实践中学习随机规划、滚动状态反馈、Python 与实验分析；AI 辅助产出与个人独立掌握程度分别描述，不使用无依据的熟练度标签。
- 工作方式依据用户表达的偏好：追问原理、重视证据、偏好简洁可复用实现。Big Five 保留原嵌入，不推断分数或人格类型。
- 保持 Chen LM 与现有脱敏设置，不恢复真实姓名、学校名称、照片、手机号或个人邮箱，不公开私有研究仓库的本地证据路径或运行授权文件。

## 本地运行

需要 Node.js 24 或兼容版本。

```bash
npm ci
npm run dev
```

构建静态页面：`npm run build`，输出至 `dist/`。

## GitHub Pages

将源码推送到 `Brolem/Brolem.github.io` 仓库的 `main` 分支，在仓库 **Settings → Pages → Build and deployment → Source** 选择 **GitHub Actions**。项目内的 `.github/workflows/deploy.yml` 会在推送时构建和部署。网站地址为 `https://brolem.github.io/`。

首页：`src/pages/index.astro`；研究案例：`src/pages/projects/bilateral-uncertainty.astro`；共用样式：`src/styles/global.css`。研究进度变化时，同步更新首页状态、案例页的阶段验证、结果与结论边界，并重新核对学习阶段。
