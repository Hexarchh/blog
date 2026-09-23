# Chen Kai 的博客

我的个人博客，记录学习、思考与生活。

- **线上地址**：待部署
- **源码**：[github.com/Hexarchh/blog](https://github.com/Hexarchh/blog)
- **技术栈**：[Astro](https://astro.build/) + [AstroPaper](https://github.com/satnaing/astro-paper) 主题（感谢作者的 MIT 开源）

## 本地开发

```bash
pnpm install   # 安装依赖
pnpm dev       # 启动本地预览 http://localhost:4321
pnpm build     # 构建静态站点到 dist/
```

## 目录速查

| 路径 | 用途 |
|---|---|
| `astro-paper.config.ts` | 站点标题、作者、社交链接等核心配置 |
| `src/content/posts/` | 博客文章（Markdown） |
| `src/content/pages/` | 独立页面（关于页等） |
| `src/i18n/lang/` | 界面文案翻译 |

## 写新文章

在 `src/content/posts/` 下新建 `.md` 文件，文件头部使用如下 frontmatter：

```yaml
---
author: Chen Kai
pubDatetime: 2026-09-23T09:00:00Z
title: 文章标题
slug: url-friendly-slug
featured: false
draft: false
tags:
  - 标签
description: 一句话摘要
---
```
