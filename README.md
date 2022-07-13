# Lous

[![license](https://img.shields.io/github/license/liuxiaotian/hexo-theme-lous?style=flat-square)](https://github.com/liuxiaotian/hexo-theme-lous/blob/main/LICENSE)
[![hexo-version](https://img.shields.io/badge/hexo-5.0+-0E83CD?style=flat-square&logo=hexo)](https://hexo.io/)
[![node-version](https://img.shields.io/badge/node-10.13+-339933?style=flat-square&logo=node.js)](https://nodejs.org/en/)
[![prs-welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square&logo=github)](https://github.com/liuxiaotian/hexo-theme-lous/pulls)

一款极简的 Hexo 主题，其名出自刘禹锡的《陋室铭》：“斯是陋室，惟吾德馨”。

预览：[我的博客](https://liuxiaotian.com)

## 配置

在根目录下创建 `_config.lous.yml`。

``` yml
# 配置 favicon，目录位于 source 文件夹下
favicon: images/avatar.png

# 顶部菜单
menu:
  主页: /
  关于: about

# 版权说明
copyright:
  name: yourname

# 文章协议
license:
  name: CC-BY-NC-SA 4.0
  url: https://creativecommons.org/licenses/by-nc-sa/4.0/

# rss
rss:
  path: atom.xml
  # path: rss2.xml

# MathJax
mathjax:
  enable: false
  # cnd: https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-svg.min.js

# KaTeX
# 移除默认的渲染器：
# $ npm uninstall hexo-renderer-marked --save
# 安装：
# $ npm install @upupming/hexo-renderer-markdown-it-plus --save
# 安装完成后执行清理命令：
# $ hexo clean
katex:
  enable: false
  # cdn: https://cdn.jsdelivr.net/npm/katex@0/dist/katex.min.css

# 评论系统：Utterances
utterances:
  enable: true
  repo: owner/repo
  issueTerm: pathname
  theme: github-light

# 谷歌分析
analytics:
  enable: true
  gtag: G-XXXXXXXXXXXX
```

### RSS

需安装插件 `hexo-generator-feed`，请参考 [hexo-generator-feed](https://github.com/hexojs/hexo-generator-feed)。

### 代码高亮

启用站点配置中的 `hljs`。

``` yml
highlight:
  enable: true
  line_number: false
  auto_detect: false
  tab_replace: ''
  wrap: false
  hljs: true
```
