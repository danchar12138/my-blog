---
title: Danchar-Blog部署指南
abbrlink: b6cb746c
date: 2023-11-08 12:54:15
categories: [博客相关]
tags: [Hexo, Butterfly]
---
# Danchar's Blog

基于hexo框架，以及butterfly主题的个人博客项目。

## 网站部署

### hexo快速部署

```bash
npm install hexo-cli -g
hexo init blog
cd blog
npm install
hexo server
```

### butterfly快速部署

克隆butterfly项目

```bash
git clone -b master https://gitee.com/immyw/hexo-theme-butterfly.git themes/butterfly
```

安装主题所需依赖

```bash
npm install hexo-renderer-pug hexo-renderer-stylus --save
```

### github pages快速部署

首先新建一个名称为 `yourname.github.io` 的仓库

若本地仓库已存在

```bash
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/yourname/project.git
git push -u origin main
```

若本地仓库不存在

```bash
git remote add origin https://github.com/yourname/project.git
git branch -M main
git push -u origin main
```

## 操作命令

### 文章

```bash
hexo new 文章标题
```

### 推送

推送网站到github pages仓库

```bash
hexo clean
hexo generate
hexo deploy
```

本地运行静态网站

```
hexo server
```

### 迁移

从 RSS 迁移所有文章。`source` 可以是文件路径或网址。

```bash
hexo migrate rss <source>
```

## 补充说明

待补充
