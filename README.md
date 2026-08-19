# PyClaw 官网

**一个 Agent,走遍天下。**

PyClaw 的官方网站,单文件静态站点,零构建。

## 本地预览

直接用浏览器打开 `index.html`,或起个静态服务:

```bash
npx serve .
```

## 部署到 Cloudflare Pages

1. 在 Cloudflare Dashboard 创建 Pages 项目,连接本仓库
2. 构建配置:
   - **构建命令**:留空(纯静态,无需构建)
   - **输出目录**:`/`
3. 保存即部署,每次 push 自动更新

## 技术栈

- 纯 HTML + CSS + JS,单文件
- 深色主题 · 彩色光晕背景 · 弹簧动效
- 无任何框架与构建依赖

© 2026 Campus & His OpenClaw · GPL v3.0
