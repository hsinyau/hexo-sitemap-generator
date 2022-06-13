# hexo-sitemap-generator

Sitemap generator plugin for Hexo, Changes in the [hexo-generator-sitemap](https://www.npmjs.com/package/hexo-generator-sitemap)

Support: `.xml`、`.txt`、`.html` 

## Install

``` bash
$ npm install hexo-sitemap-generator --save
```

## Options

You can configure this plugin in `_config.yml`.

``` yaml
sitemaps:
  path: 
    - sitemap.xml
    - sitemap.txt
    - sitemap.html
  # template: ./sitemap_template.xml
  # template_txt: ./sitemap_template.txt
  # template_html: ./sitemap_template.html
  rel: false
  tags: true
  categories: true
```

- **path** - Sitemap path. (Default: sitemap.xml)
- **template** - Custom template path. This file will be used to generate sitemap.xml (See [default xml template](/sitemap.xml))
- **template_txt** - Custom template path. This file will be used to generate sitemap.txt (See [default txt template](/sitemap.txt))
- **template_html** - Custom template path. This file will be used to generate sitemap.html (See [default html template](/sitemap.html))
- **rel** - Add [`rel-sitemap`](http://microformats.org/wiki/rel-sitemap) to the site's header. (Default: `false`)
- **tags** - Add site's tags
- **categories** - Add site's categories

## Exclude Posts/Pages

Add `sitemap: false` to the post/page's front matter.

``` yml
---
title: lorem ipsum
date: 2020-01-02
sitemap: false
---
```
