# flat-ghost
[English](README.md) | 中文

一个响应式设计的扁平化风格 **Ghost v5.x** 博客主题，[主题预览](https://blog.avinzheng.com)。


## 安装

前往 [releases](https://github.com/avinzheng/ghost-theme-flat-ghost/releases) 页面下载最新版 zip 安装包，登录 Ghsot 博客管理后台上传并启用主题。

## 特点

*   主题内置多个配色方案，支持 7 种配色方案切换；
*   移动设备采用安卓风格侧滑菜单（仿 Ionic 3 on Android）；
*   内置常见编程语言代码高亮（by Prism）；
*   侧边栏多种小工具支持（推荐文章、标签、博客统计、关注）；
*   额外的社会化链接图标：GitHub、LinkedIn、知乎、微博、微信、QQ 。

## 自定义

### 切换主题颜色

打开主题 `default.hbs` 文件，在 body 标签中设置主题颜色类名，支持以下颜色类名：

* `theme-turquoise` （默认）
* `theme-blue`
* `theme-green`
* `theme-red`
* `theme-orange`
* `theme-yellow`
* `theme-purple`

### 设置社会化链接

打开主题 `partials/widget-blog-follow.hbs` 文件，找到如下代码，根据需要修改。

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

