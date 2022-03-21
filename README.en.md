<div align="right">
  🌏 <a title="Chinese" href="README.md">简体中文</a> | English
</div>

# Lous

[![license](https://img.shields.io/github/license/liuxiaotian/hexo-theme-lous?style=flat-square)](https://github.com/liuxiaotian/hexo-theme-lous/blob/main/LICENSE)
[![hexo-version](https://img.shields.io/badge/hexo-5.0+-0E83CD?style=flat-square&logo=hexo)](https://hexo.io/)
[![node-version](https://img.shields.io/badge/node-10.13+-026E00?style=flat-square&logo=node.js)](https://nodejs.org/en/)
[![prs-welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square&logo=github)](https://github.com/liuxiaotian/hexo-theme-lous/pulls)

Lous is a ~~crude~~ minimalist theme. Its name comes from a poetry 'Loushi Ming' by the ancient Chinese poet [Liu Yuxi](https://en.wikipedia.org/wiki/Liu_Yuxi). It means that poverty does not limit one's spiritual abundance.

## Preview

![preview](/source/_images/screenshot.png)

My blog: [liuxiaotian.com](https://liuxiaotian.com)

## Installation

You can clone this repo:

``` bash
$ cd hexo-site
$ git clone https://github.com/liuxiaotian/hexo-theme-lous.git themes/next
```

Or add this repo as a submodule:

``` bash
$ cd hexo-site
$ git submodule add https://github.com/liuxiaotian/hexo-theme-lous.git themes/next
```

After the installation, edit the site configuration, set the `theme` variable to `lous`.

``` yml
theme: next
```

## Configuration

Create a file named `_config.lous.yml` and place it at the same level as the site configuration.

``` yml
# Configure favicon, the directory is located under the source folder
favicon: images/avatar.png

# Top menu (No configure, no display)
menu:
  Home: /
  About: about

# Copyright (No configure, no display)
copyright:
  name: yourname

# The license of articles (No configure, no display)
license:
  name: CC-BY-NC-SA 4.0
  url: https://creativecommons.org/licenses/by-nc-sa/4.0/

# rss (No configure, no display)
rss:
  path: atom.xml
  # path: rss2.xml

# MathJax
mathjax:
  enable: false
  showPageOnRenderFinish: true 
  timeout: 1000 # Show page after 1000ms, even if mathjax doesn't finish rendering

# Utterances is a lightweight comments widget built on GitHub issues. See https://utteranc.es/
utterances:
  enable: true
  repo: owner/repo
  issueTerm: pathname
  theme: github-light
```

### RSS

RSS requires `hexo-generator-feed` to be installed in the site root.

For this plugin's installation and configuration, please check [https://github.com/hexojs/hexo-generator-feed](https://github.com/hexojs/hexo-generator-feed).

### Highlight

To enable highlight you need to enable `hljs` in the site configuration. At the same time, a space should be added between the backticks and the language identifier.

``` yml
highlight:
  enable: true
  line_number: false
  auto_detect: false
  tab_replace: ''
  wrap: false
  hljs: true
```
