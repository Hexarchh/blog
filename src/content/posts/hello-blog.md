---
author: Hexarchh
pubDatetime: 2026-09-23T09:00:00Z
title: 你好，世界：这个博客开张了
slug: hello-blog
featured: true
draft: false
tags:
  - 随笔
  - 建站
description: 从挑选模板到推送 GitHub，记录这个博客诞生的全过程。
---

想了很久要有个自己的写字的地方，今天终于动手了。这篇文章记录一下搭建的全过程，也当是博客的开工纪念。

## 为什么自己搭博客

平台上的内容终究是寄人篱下，广告、算法、关闭的服务，哪一样都让人不踏实。自己的博客，数据在自己手里，写什么、长什么样，都自己说了算。

## 搭建过程

整个流程其实比想象中简单，总共四步：

1. **挑模板**：在 GitHub 上按 Star 数和维护活跃度筛选，最终选了 [AstroPaper](https://github.com/satnaing/astro-paper) —— 5000+ Star，维护活跃，极简风格，SEO 友好，而且文档很完整
2. **克隆到本地**：`git clone` 一条命令，再用 pnpm 装好依赖
3. **本地预览**：`pnpm dev` 起一个本地服务器，浏览器打开 `localhost:4321` 实时看效果
4. **推送 GitHub**：删掉模板自带的 git 历史，初始化自己的仓库，推送到 [Hexarchh/blog](https://github.com/Hexarchh/blog)

Astro 框架的体验不错：构建快、默认输出纯静态页面，加载速度飞快，对搜索引擎也友好。

## 接下来

- 把博客部署上线，让别人也能访问
- 慢慢把这里填满：技术笔记、生活记录、乱七八糟的想法
- 折腾一下主题细节，让它更像「我的」地方

万里长征第一步，先写到这里。
