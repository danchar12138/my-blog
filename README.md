# Danchar's Blog

基于hexo框架，以及butterfly主题的个人博客项目。

## hexo快速部署

```bash
npm install hexo-cli -g
hexo init blog
cd blog
npm install
hexo server
```

## butterfly快速部署

克隆butterfly项目

```bash
git clone -b master https://gitee.com/immyw/hexo-theme-butterfly.git themes/butterfly
```

安装主题所需依赖

```bash
npm install hexo-renderer-pug hexo-renderer-stylus --save
```

## github pages快速部署

新建仓库 `yourname.github.io`

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

## 补充说明

待补充
