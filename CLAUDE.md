# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目简介

一个极简的手写静态网站，通过 GitHub Pages 部署在 `baiqiantao.github.io`。包含两个独立的 HTML 文件，无构建系统、无框架、无依赖。内容和注释均为中文。

## 文件说明

- `index.html` — 个人主页（纯 HTML + CSS，无 JS）
- `heartbeat.html` — 互动动画作文展示页面，支持语音朗读、逐字显示动画和字体切换。引用了 `bgm.mp3`（未纳入仓库）。

## 开发方式

无需构建步骤。直接编辑 HTML 文件，推送到 `master` 分支即可通过 GitHub Pages 部署。

```bash
# 本地预览
open index.html

# 部署
git add index.html heartbeat.html
git commit -m "描述信息"
git push origin master
```

## 已知问题

- `index.html` 的 favicon 指向 `/hexoBlog/favicon.png`（旧的 Hexo 路径，已失效）
- `heartbeat.html` 引用了 `bgm.mp3`，但该文件未纳入仓库管理
