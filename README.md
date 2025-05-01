# flat-ghost

English | [中文](README_zh-CN.md)

A responsive, flat-design **Ghost v5.x** blog theme. [Theme Preview](https://blog.avinzheng.com/).

## Installation

Go to the [releases](https://github.com/avinzheng/ghost-theme-flat-ghost/releases) page to download the latest version of the zip package. Log in to your Ghost blog admin panel, upload the theme, and activate it.

## Features

- Built-in multiple color schemes, supporting 7 switchable color options.
- Android-style sliding menu for mobile devices (inspired by Ionic 3 on Android).
- Built-in syntax highlighting for common programming languages (powered by Prism).
- Multiple sidebar widgets supported (featured posts, tags, blog statistics, follow section).
- Additional social media link icons: GitHub, LinkedIn, Zhihu, Weibo, WeChat, QQ.

## Customization

### Switching Theme Colors

Open the theme's `default.hbs` file and set the theme color class name in the body tag. The following color class names are supported:

- `theme-turquoise` (default)
- `theme-blue`
- `theme-green`
- `theme-red`
- `theme-orange`
- `theme-yellow`
- `theme-purple`

### Setting Up Social Links

Open the theme's `partials/widget-blog-follow.hbs` file and locate the following code. Modify it as needed.

```html
  <ul class="social">
<!--    <li>-->
<!--      <a href="https://github.com/avincheng/ghost-theme-flatghost"-->
<!--         title="GitHub"-->
<!--         target="_blank"-->
<!--         rel="noopener">-->
<!--        <i class="icon-social icon-social-github"></i>-->
<!--      </a>-->
<!--    </li>-->

    {{#if @site.facebook}}
      <li>
        <a href="{{facebook_url}}"
           title="FaceBook"
           target="_blank"
           rel="noopener">
          <i class="icon-social icon-social-facebook"></i>
        </a>
      </li>
    {{/if}}

    {{#if @site.twitter}}
      <li>
        <a href="{{twitter_url}}"
           title="Twitter"
           target="_blank"
           rel="noopener">
          <i class="icon-social icon-social-twitter"></i>
        </a>
      </li>
    {{/if}}

<!--    <li>-->
<!--      <a href=""-->
<!--         title="LinkedIn"-->
<!--         target="_blank"-->
<!--         rel="noopener">-->
<!--        <i class="icon-social icon-social-linkedin"></i>-->
<!--      </a>-->
<!--    </li>-->

<!--    <li>-->
<!--      <a href=""-->
<!--         title="ZhiHu"-->
<!--         target="_blank"-->
<!--         rel="noopener">-->
<!--        <i class="icon-social icon-social-zhihu"></i>-->
<!--      </a>-->
<!--    </li>-->

<!--    <li>-->
<!--      <a href=""-->
<!--         title="WeiBo"-->
<!--         target="_blank"-->
<!--         rel="noopener">-->
<!--        <i class="icon-social icon-social-weibo"></i>-->
<!--      </a>-->
<!--    </li>-->

<!--    <li>-->
<!--      <a href=""-->
<!--         title="WeChat"-->
<!--         target="_blank"-->
<!--         rel="noopener">-->
<!--        <i class="icon-social icon-social-wechat"></i>-->
<!--      </a>-->
<!--    </li>-->

<!--    <li>-->
<!--      <a href=""-->
<!--         title="QQ"-->
<!--         target="_blank"-->
<!--         rel="noopener">-->
<!--        <i class="icon-social icon-social-qq"></i>-->
<!--      </a>-->
<!--    </li>-->
  </ul>
```

