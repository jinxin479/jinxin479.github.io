---
layout: post
title: "利用Jekyll搭建博客"
date: "2015-11-01"
slug: "利用Jekyll搭建博客"
id: "20151101"
description: "将纯文本转换为静态博客网站，不再需要数据库，不需要开发评论功能，不需要不断的更新版本——只用关心你的博客内容。使用Markdown（或 Textile）、Liquid 和 HTML & CSS 构建可发布的静态网站将纯文本转换为静态博客网站，不再需要数据库，不需要开发评论功能，不需要不断的更新版本——只用关心你的博客内容。使用Markdown（或 Textile）、Liquid 和 HTML & CSS 构建可发布的静态网站."
category:
  - views
  - featured
# tags will also be used as html meta keywords.
tags:
  - 博客
  - Jekyll
show_meta: true
comments: true
mathjax: true
gistembed: true
published: true
noindex: false
nofollow: false
# hide QR code, permalink block while printing.
hide_printmsg: false
# show post summary or full post in RSS feed.
summaryfeed: false
## for twitter summary card with squared image and page description or page excerpt:
# imagesummary: foo.png
## for twitter card with large image:
# imagefeature: "http://img.youtube.com/vi/VEIrQUXm_hY/0.jpg"
## for twitter video card: (active for this page)
---

将纯文本转换为静态博客网站，不再需要数据库，不需要开发评论功能，不需要不断的更新版本——只用关心你的博客内容。

<!--more-->

## 安装Ruby环境
&emsp;&emsp;安装完成Jekyll可能需要花几分钟的时间，但非常简单。请确保你在系统里已经有如下配置。

* Ruby（including development headers, Jekyll 2 需要 v1.9.3 及以上版本，Jekyll 3 需要 v2 及以上版本）
* RubyGems
*  Linux, Un ix, or Mac OS X
* NodeJS, 或其他 JavaScript 运行环境（Jekyll 2 或更早版本需要 CoffeeScript 支持）。
* Python 2.7（Jekyll 2 或更早版本）
安装地址: http://rubyinstaller.org/downloads/,   mac直接去官网下载

## 安装Jekyll

&emsp;&emsp;安装 Jekyll 的最好方式就是使用 RubyGems. 你只需要打开终端输入以下命令就可以安装了：
使用 `gem install jekyll` 命令安装jekyll

## 使用Jekyll
&emsp;&emsp;创建博客目录，随便命名，如：my-site
{% highlight bash %}
~ $ jekyll new my-site  
~ $ cd my-site
~/my-site $ bundle install
~/my-site $ bundle exec jekyll serve
{% endhighlight %}

一个基本的 Jekyll 网站的目录结构一般是像这样的：
![目录结构]({{ site.urlimg }}/media/jekyll-04.png "目录结构")
来看看目录的详细介绍吧：
![目录结构]({{ site.urlimg }}/media/jekyll-05.png "目录结构")
打开浏览器在地址栏输入： http://localhost:4000，就可以看到效果了，是不是很爽啊！
- *注意*：这几部有可能出错，如果说是该端口已经被绑定了，此时需要你手动到配置文件中修改，换一个端口。在 `_confit.yml`文件中增加：port:2000
![端口错误]({{ site.urlimg }}/media/jekyll-01.png "端口错误")
如果是bundle 不是内部命令
![错误]({{ site.urlimg }}/media/jekyll-02.png "错误")
请敲入命令`gem install bundle`安装bundle可以解决

## 选择模板
&emsp;&emsp;使用Jekyll的好处就是有很多模板可以使用，免去自己构建页面的繁琐事情。
模板网址：[Jkeyll主题](http://jekyllthemes.org/)  选择自己喜欢的风格下载下来使用吧！
在使用模板的时候，可以更改`_config.yml`文件中的配置，比如网站地址，标题等等。怎么样，是不是很强大。
![模板]({{ site.urlimg }}/media/jekyll-06.png "模板")

## 使用模板
&emsp;&emsp;安装过程比较简单，通过git clone将模板代码下载到本地目录中。运行`bundle install`进行依赖包安装（原理类似于python的virtualenv）。然后用`bundle exec jekyll serve`就可以查看模板效果了。不建议通过`jekyll serve`命令启动jekyll,很容易出错。模板是通过bundle安装独立的依赖包环境的，因此一定需要通过`bundle exec jekyll serve`才能够使用到本目录下的依赖环境正常运行

## 博客发布
&emsp;&emsp;Github Pages 是面向用户、组织和项目开放的公共静态页面搭建托管服 务，站点可以被免费托管在 Github 上，你可以选择使用 Github Pages 默 认提供的域名 github.io 或者自定义域名来发布站点。Github Pages 支持 自动利用 Jekyll 生成站点，也同样支持纯 HTML 文档，将你的 Jekyll 站 点托管在 Github Pages 上是一个不错的选择。
假如你还不清楚怎么使用Github Pages 请点击[github-pages介绍](http://jmcglone.com/guides/github-pages/).
在github上新建一个仓库，命名为username.github.io username是你的github用户名。把该仓库克隆到本地，把你的项目放到仓库所在文件夹中，如果模板中存在.git文件请先删除。然后最重要的一步：把项目推送到github上，访问username.github.io就可以看你的博客啦！

### 参考
[Jkeyll官网中文](http://jekyllcn.com/docs/home/)
[Jkeyll主题](http://jekyllthemes.org/)
