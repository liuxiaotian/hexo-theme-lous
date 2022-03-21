<div align="right">
  🌏 简体中文 | <a title="English" href="README.en.md">English</a>
</div>

# Lous

[![license](https://img.shields.io/github/license/liuxiaotian/hexo-theme-lous?style=flat-square)](https://github.com/liuxiaotian/hexo-theme-lous/blob/main/LICENSE)
[![hexo-version](https://img.shields.io/badge/hexo-5.0+-0E83CD?style=flat-square&logo=hexo)](https://hexo.io/)
[![node-version](https://img.shields.io/badge/node-10.13+-339933?style=flat-square&logo=node.js)](https://nodejs.org/en/)
[![prs-welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square&logo=github)](https://github.com/liuxiaotian/hexo-theme-lous/pulls)

Lous 是一款~~简陋~~极简的 Hexo 主题。其名出自刘禹锡的《陋室铭》：“斯是陋室，惟吾德馨”。

## 预览

![preview](/source/_images/screenshot.png)

我的博客：[liuxiaotian.com](https://liuxiaotian.com)

## 安装

克隆本仓库：

``` bash
$ cd hexo-site
$ git clone https://github.com/liuxiaotian/hexo-theme-lous.git themes/next
```

或者添加子模块：

``` bash
$ cd hexo-site
$ git submodule add https://github.com/liuxiaotian/hexo-theme-lous.git themes/next
```

完成后，将站点配置 `theme` 改为 `lous`。

``` yml
theme: next
```

## 配置

在站点配置同级目录下创建 `_config.lous.yml`。

``` yml
# 配置 favicon，目录位于 source 文件夹下
favicon: images/avatar.png

# 顶部菜单（不配置则不显示）
menu:
  主页: /
  关于: about

# 版权说明（不配置则不显示）
copyright:
  name: yourname

# 文章协议（不配置则不显示）
license:
  name: CC-BY-NC-SA 4.0
  url: https://creativecommons.org/licenses/by-nc-sa/4.0/

# rss (不配置则不显示)
rss:
  path: atom.xml
  # path: rss2.xml

# MathJax
mathjax:
  enable: false
  showPageOnRenderFinish: true # MathJax 渲染完成才显示页面
  timeout: 1000 # 1000 毫秒后显示页面，即使 mathjax 没有渲染完成

# Utterances 是一个基于 GitHub Issues 的轻量级评论系统。请查看 https://utteranc.es/
utterances:
  enable: true
  repo: owner/repo
  issueTerm: pathname
  theme: github-light
```

### RSS

RSS 功能需要在站点根目录下安装插件 `hexo-generator-feed`。

该插件的安装和配置说明见 [https://github.com/hexojs/hexo-generator-feed](https://github.com/hexojs/hexo-generator-feed)。

### 代码高亮

代码高亮需要启用站点配置中的 `hljs`，同时 Markdown 中代码块开头的语言与反引号之间应该添加空格。

``` yml
highlight:
  enable: true
  line_number: false
  auto_detect: false
  tab_replace: ''
  wrap: false
  hljs: true
```
