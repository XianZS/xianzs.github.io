---
title: Tailwind CSS使用指南
date: 2026-01-28
---

# Tailwind CSS使用指南

## 什么是Tailwind CSS？

Tailwind CSS是一个实用优先的CSS框架，它提供了大量的原子类，让你可以直接在HTML中构建自定义界面，而不需要编写传统的CSS。

## Tailwind CSS的特点

- **实用优先**：提供了大量的原子类，如`flex`、`p-4`、`text-center`等
- **高度可定制**：可以通过配置文件自定义主题、颜色、字体等
- **响应式设计**：内置响应式类，如`md:flex`、`lg:text-xl`等
- **无冗余CSS**：只生成你使用的类，减少CSS文件大小
- **开发效率高**：不需要在HTML和CSS之间切换，直接在HTML中编写样式

## 基本使用

### 安装

```bash
npm install -D tailwindcss postcss autoprefixer
```

### 初始化配置

```bash
npx tailwindcss init -p
```

### 配置内容路径

在`tailwind.config.js`中配置内容路径：

```js
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./**/*.{html,js,ts,vue,md}"
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

### 在CSS中引入Tailwind

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

## 常用类

### 布局类

- `flex`：弹性布局
- `grid`：网格布局
- `block`：块级元素
- `inline`：行内元素

### 间距类

- `p-4`：内边距4
- `m-2`：外边距2
- `mt-4`：上外边距4
- `mb-6`：下外边距6

### 文本类

- `text-center`：文本居中
- `text-xl`：文本大小xl
- `font-bold`：字体加粗
- `text-blue-500`：文本颜色蓝色500

### 响应式类

- `md:flex`：在中等屏幕以上使用弹性布局
- `lg:text-xl`：在大屏幕以上使用xl文本大小
- `sm:grid-cols-2`：在小屏幕以上使用2列网格

## 自定义主题

你可以在`tailwind.config.js`中自定义主题：

```js
export default {
  theme: {
    extend: {
      colors: {
        primary: '#3b82f6',
        secondary: '#f59e0b',
      },
      fontFamily: {
        sans: ['Inter', 'sans-serif'],
      },
    },
  },
}
```

## 总结

Tailwind CSS是一个非常强大的CSS框架，它改变了我们编写CSS的方式，让我们可以更快速、更灵活地构建现代化的界面。如果你还没有尝试过Tailwind CSS，我强烈建议你给它一个机会！