# PyClaw 官网

**一个 Agent,走遍天下。**

PyClaw 的官方网站,**双站并存,纯静态,零构建**。

## 站点结构

```
/                 → PyClaw 主站(index.html)
/lite/index.html  → PyClaw Lite 官网
```

- **主站** `index.html`:完整版 PyClaw —— 三种模式、8 插件 / 36+ 工具、多 Agent 架构。
- **Lite 站** `lite/index.html`:轻量分支 —— 2854 行 Python、一个 `exec`、一个依赖。
- 两站互链:主站导航 / Lite 板块 / 页脚 → Lite 站;Lite 站导航 / Hero / 交叉横幅 → 主站。

## 本地预览

直接用浏览器打开 `index.html`,或起个静态服务:

```bash
npx serve .
```

然后访问 `/` 与 `/lite/`。

## 部署到 Cloudflare Pages

1. 在 Cloudflare Dashboard 创建 Pages 项目,连接本仓库
2. 构建配置:
   - **构建命令**:留空(纯静态,无需构建)
   - **输出目录**:`/`
3. 保存即部署,每次 push 自动更新

## 技术栈

- 纯 HTML + CSS + JS,无任何框架与构建依赖
- 深色主题 · 彩色光晕背景 · 弹簧动效 · 视差光晕 · 打字机终端 · 无限跑马灯 · Bento 卡片
- 共享同一套设计 token(颜色 / 圆角 / 缓动 / 字体),Lite 站以青绿 `--accent` 区分主站的蓝色 `--brand`

## 维护注意

- 改 Lite 相关文案/截图时,**两处都要改**:主站 `#lite` 板块与 `lite/index.html`。
- Lite 版本号当前为 `v0.0.1-beta.2`,来源 `D:\pyclaw-lite\pyclaw\__init__.py` 的 `VERSION`。
- Lite 的能力数据(2854 行 / 12 模块 / 1 依赖 / 12 钩子事件 / 20+ 供应商)以 `D:\pyclaw-lite` 仓库为准。

© 2026 Campus & His OpenClaw · GPL v3.0
