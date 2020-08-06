# Theme: Materialized

A cool materialized theme for [Hexo](https://hexo.io/).

View the demo site [here](https://theme-materialized.github.io).

## Screenshots

![frontpage](https://i.loli.net/2019/08/12/8fKedcbWDkpCqEI.png)

![post](https://i.loli.net/2019/08/12/2faKWNcsXMC8OAh.png)

![comments](https://i.loli.net/2019/08/12/UcJH3BsXK4Ax7aV.png)

![search](https://i.loli.net/2019/08/12/r4pZfcNshxQaw6k.png)

![darkmode](https://i.loli.net/2019/08/12/MKvX3Iq8T7SrH6Z.png)

## Installation

### Install

``` bash
$ git clone https://github.com/theme-materialized/hexo-theme-materialized themes/materialized
```

### Enable

Modify `theme` setting in `_config.yml` of the site to `materialized`.

## Configuration

### `_config.yml` file under `/themes/materialized/`

``` yml
theme_color: # Theme color. Please go to [Colors](https://www.mdui.org/docs/color)
  primary: indigo
  accent: pink

notice: # Notice or announcement. Support `<a>` tag

favicon: /images/favicon.png # Favicon path
banner: /images/banner.png # Sidebar background image path
avatar: /images/avatar.png # Avatar image path
rss: /atom.xml # RSS link. `hexo-generator-feed` plugin is needed

email: # Email address
sns: # SNS links
  twitter:
  facebook:
  google_plus:
  weibo:
  instagram:
  tumblr:
  github:
  linkedin:
  zhihu:
  douban:
  qq:
  wechat:

open_graph: # OpenGraph settings
  twitter:
  google_plus:
  fb_admins:
  fb_app_id:
site_verification: # Site verification keys
  google:
  baidu:
analytics: # Site analytics IDs
  google_site_id:
  baidu_site_id:
  cnzz_site_id:
pages: # Custom page links. Set with `name` and `link`
- name: Tags
  link: /tags
- name: Gallery
  link: /gallery
links: # Friendship links. Set with `name` and `link`
- name: Github
  link: https://github.com

since: 2019 # Start year, use a 4-digit number. If you don't set the start year, there won't be a "since xxxx" on the bottom of your site
footer_text: # Additional text in footer, such as the record information. Support `<a>` tag
license: # License description of every article. Support `<a>` tag

gallery: # CDN links of `fancybox` plugin used on Gallery page
  fancybox_css: https://cdn.bootcss.com/fancybox/3.5.7/jquery.fancybox.min.css
  fancybox_js: https://cdn.bootcss.com/fancybox/3.5.7/jquery.fancybox.min.js
  jquery_js: https://cdn.bootcss.com/jquery/3.3.1/jquery.min.js
  lazyload_js: https://cdn.bootcss.com/jquery_lazyload/1.9.7/jquery.lazyload.min.js
busuanzi: # Use `busuanzi` plugin to count website visits
  site: false
  page: false
  busuanzi_js: http://busuanzi.ibruce.info/busuanzi/2.3/busuanzi.pure.mini.js
qrcode: # Qrcode for articles. if use `plugin`, `hexo-helper-qrcode` plugin is needed
  caption: Send to mobile phone
  use: plugin
donate: # Use your payment qrcode or link to receive donations. Set with `name` and `link`
search: # Search settings. if use `plugin`, `hexo-generator-search` plugin is needed and `path` should be set correctly
  placeholder: Enter key words
  path: /search.xml
  use: plugin
comment: # Comment plugin settings. Set `use` with the plugin name such as `gitalk`
  use: false
  disqus_shortname:
  gitalk_client_id:
  gitalk_client_secret:
  gitalk_repo:
  gitalk_owner:
  livere_data_uid:
  valine_leancloud_app_id:
  valine_leancloud_app_key:
  valine_placeholder:
  valine_page_size:
  valine_avatar:
  valine_lang:
  valine_guest_info:
  valine_notify:
  valine_verify:
  changyan_app_id:
  changyan_app_key:
  changyan_sid_type:
```

### Article/Page Front-matter

``` yml
thumbnail: /xxx.jpg  # Custom page header image.
author: xxx  # Author.
categories: [xxx]  # Categories. Support more than one categories.
tags:  # Tags.
  - xxx
qrcode: false  # Disable article qrcode.
share_menu: false  # Disable article share menu.
license: xxx  # License description of the article.
donate: false  # Disable article donate link.
toc: true  # Enable article toc.
comments: true  # Enable article comment.
```

## Sample Article

```markdown
---
title: Sample Article
categories: [Test]
tags:
  - Tag1
  - Tag2
author: Test
comments: false
---

Write something here...
```

If `thumbnail` in Article/Page Front-matter is not set, a random image will be used.

If `author` in Article/Page Front-matter is not set, `author` in site `_config.yml` will be used.

Also, `toc`, `comments`, `qrcode`, `share_menu` and `donate` is enabled by default if you chose to enable them in the theme `_config.yml`.
