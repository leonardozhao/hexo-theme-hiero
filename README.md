# Hiero

[![Build Status](https://travis-ci.org/iTimeTraveler/hexo-theme-hiero.svg?branch=master)](https://travis-ci.org/iTimeTraveler/hexo-theme-hiero)		[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/iTimeTraveler/hexo-theme-hiero/blob/master/LICENSE)


Hiero is an awesome magazine theme for your [Hexo] site.

[**☞ Live Preview**](https://itimetraveler.github.io/hexo-theme-hiero/)  |  [**✎ Hiero 中文使用文档**](https://github.com/iTimeTraveler/hexo-theme-hiero/blob/master/README.cn.md)

![](https://raw.githubusercontent.com/iTimeTraveler/hexo-theme-hiero/master/source/preview/Hiero_home.png)

<!--more-->

## Installation

 1. Get it from GitHub

 ```shell
 $ git clone https://github.com/iTimeTraveler/hexo-theme-hiero.git themes/hiero
 ```
 2. Enable

 Modify `theme` setting in `_config.yml` to `hiero`.
 ```
 # Extensions
 ## Plugins: http://hexo.io/plugins/
 ## Themes: http://hexo.io/themes/
 theme: hiero
 ```
 3. Update

 ```shell
 $ cd themes/hiero
 $ git pull
 ```


## Features


### Code Highlight

Hiero use [Tomorrow Theme](https://github.com/chriskempson/tomorrow-theme) for your code block. We have six options in total: `default`, `normal`, `night`, `night blue`, `night bright`, `night eighties`

![code `default` theme Preview](https://itimetraveler.github.io/hexo-theme-hiker/2016/10/24/Hiker%E4%B8%BB%E9%A2%98%E9%A2%84%E8%A7%88/code-theme-default.png)

Above preview picture is default theme. the image below show other five Highlight themes.

![code themes](https://github.com/iTimeTraveler/hexo-theme-hiero/blob/master/source/preview/code-theme.jpg?raw=true)

Modify `highlight_theme` in hiero/_config.yml.

```yml
# Code Highlight theme
# Available value:
#    default | normal | night | night eighties | night blue | night bright
# https://github.com/chriskempson/tomorrow-theme
highlight_theme: default
```



### Sidebar

You can put your sidebar in left side, right side or bottom of your site by editing `sidebar` setting.
Hiero provides 7 built-in widgets:

- search
- social
- recent_posts
- category
- tag
- tagcloud
- archive

All of them are enabled by default. You can edit them in `widget` setting.


### Search

Hiero use `Insight Search` to help you search anything inside your site without any third-party plugin.

```yml
# Search
search:
    insight: true # you need to install `hexo-generator-json-content` before using Insight Search
    swiftype: # enter swiftype install key here
    baidu: false # you need to disable other search engines to use Baidu search, options: true, false
```

> Attention: You need to install `hexo-generator-json-content` before using Insight Search.

```bash
$ npm install -S hexo-generator-json-content
```


### Fancybox

Hiero uses [Fancybox] to showcase your photos. You can use Markdown syntax or fancybox tag plugin to add your photos.

```
![img caption](img url)

{% fancybox img_url [img_thumbnail] [img_caption] %}
```

### Comment support

Hiero has native support for DuoShuo & Disqus comment systems. Modify the following snippets to Hiero `hiero/_config.yml`:

```yml
# comment ShortName, you can choose only ONE to display.
duoshuo_shortname: iTimeTraveler
disqus_shortname: 
```

## Browser support

![](https://github.com/iTimeTraveler/hexo-theme-hiero/blob/master/source/preview/browser-support.png?raw=true)


## Contributing

All kinds of contributions (enhancements, new features, documentation & code improvements, issues & bugs reporting) are welcome.

Looking forward to your pull request.


> Special thanks to ATHEMES, who designed the original theme [Hiero for Wordpress](http://athemes.com/theme/hiero/).


## License

Hiero is under the BMITSD license. See the [LICENSE](https://github.com/iTimeTraveler/hexo-theme-hiero/blob/master/LICENSE) file for details.


[Hexo]: https://hexo.io/
[Fancybox]: http://fancyapps.com/fancybox/
[Font Awesome]: http://fontawesome.io/
