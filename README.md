# 芯图相册技术博客

这是芯图相册的GitHub Pages博客，用于发布技术文章和产品更新。

## 本地开发

### 前置要求

- Ruby 2.5.0 或更高版本
- Bundler

### 安装依赖

```bash
bundle install
```

### 运行本地服务器

```bash
bundle exec jekyll serve
```

访问 http://localhost:4000 查看博客

## 部署到GitHub Pages

### 方法一：使用GitHub Actions（推荐）

1. 将代码推送到GitHub仓库
2. 在仓库设置中启用GitHub Pages
3. 选择"GitHub Actions"作为构建源
4. GitHub会自动构建和部署

### 方法二：手动部署

```bash
# 构建静态文件
bundle exec jekyll build

# 将 _site 目录的内容推送到 gh-pages 分支
```

## 添加新文章

在 `_posts` 目录中创建新文件，文件名格式：`YYYY-MM-DD-文章标题.md`

文章头部需要包含Front Matter：

```yaml
---
layout: post
title: "文章标题"
date: 2025-12-15
categories: [分类1, 分类2]
tags: [标签1, 标签2]
author: 芯图团队
---
```

## 配置自定义域名

1. 在域名DNS中添加CNAME记录：
   ```
   blog CNAME xiawenyong1977-netizen.github.io
   ```

2. 在博客根目录创建 `CNAME` 文件：
   ```
   blog.xintuxiangce.top
   ```

3. 在GitHub仓库设置中配置自定义域名

## 外链策略

本博客的所有链接都是**dofollow**，会传递SEO权重：

- ✅ 指向主网站的链接：`https://www.xintuxiangce.top`
- ✅ 指向GitHub的链接
- ✅ 指向其他相关资源的链接

**重要**：在文章中自然添加指向主网站的链接，有助于SEO优化。

## 目录结构

```
blog/
├── _config.yml          # Jekyll配置文件
├── _posts/              # 文章目录
│   └── YYYY-MM-DD-*.md
├── index.md             # 首页
├── about.md             # 关于页面
├── Gemfile              # Ruby依赖
└── README.md            # 本文件
```

## 相关链接

- [官方网站](https://www.xintuxiangce.top)
- [GitHub仓库](https://github.com/xiawenyong1977-netizen/xintuxiangce)

