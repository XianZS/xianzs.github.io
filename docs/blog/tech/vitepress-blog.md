---
title: VitePress搭建个人博客
date: 2026-01-29
---

# VitePress搭建个人博客

## 什么是VitePress？

VitePress是Vue官方推出的静态网站生成器，基于Vite和Vue 3，专门用于构建文档网站和个人博客。它具有以下特点：

- **快速的开发体验**：基于Vite的热更新，开发时响应迅速
- **简洁的Markdown支持**：内置Markdown解析和扩展
- **自动生成侧边栏**：根据目录结构自动生成导航
- **代码高亮**：支持多种编程语言的代码高亮
- **主题定制**：支持自定义主题和样式

## 为什么选择VitePress？

1. **Vue生态系统**：如果你熟悉Vue，VitePress会让你感到非常亲切
2. **静态生成**：生成的是纯静态HTML文件，加载速度快，有利于SEO
3. **GitHub Pages友好**：生成的静态文件可以直接部署到GitHub Pages
4. **内置功能丰富**：不需要安装太多插件就能满足基本需求

## 搭建步骤

### 1. 初始化项目

```bash
npm init vitepress@latest .
```

### 2. 安装依赖

```bash
npm install
```

### 3. 配置VitePress

编辑`docs/.vitepress/config.ts`文件，配置网站信息和导航

### 4. 编写内容

在`docs`目录下创建Markdown文件，编写博客内容

### 5. 构建和部署

```bash
npm run build
```

生成的文件会在`docs/.vitepress/dist`目录中，可以将其部署到GitHub Pages

## 总结

VitePress是一个非常适合搭建个人博客的工具，它简单易用，功能强大，而且与GitHub Pages完美集成。如果你正在寻找一个现代化的静态网站生成器，VitePress绝对值得尝试！