---
layout: page
permalink: /contact/
title: 联系
show_meta: false
published: true
description: "联系方式"
comments: false
mathjax: false
noindex: false
sitemap:
    priority: 0.5
    changefreq: 'monthly'
    lastmod: 2016-02-13
tags:
  - "苦瓜和尚"
  - "driving directions"
  - address
---

| <i class="fa fa-twitter"></i> | [@{{ site.owner.twitter }}](https://twitter.com/{{ site.owner.twitter }})  |
| - | :- |
| <i class="fa fa-github"></i>  | [@{{ site.owner.github }}](https://github.com/{{ site.owner.github }})  |
| - | :- |
| <i class="fa fa-instagram"></i>  |  [@{{ site.owner.instagram }}](https://instagram.com/{{ site.owner.instagram }})  |
| - | :- |
| <i class="fa fa-envelope"></i> | 金鑫<br>中国<br>北京<br>西直门   |
| - | :- |
| <i class="fa fa-paper-plane">  | jinxin479@gmail.com |
| - | :- |

<a href="https://twitter.com/share" class="twitter-share-button" data-via="{{ site.owner.twitter }}" data-size="small" data-dnt="true">Tweet</a> <a href="javascript:window.print()" class="social-icons" title="Printer friendly format"><i class="fa fa-print"></i></a>

<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+'://platform.twitter.com/widgets.js';fjs.parentNode.insertBefore(js,fjs);}}(document, 'script', 'twitter-wjs');</script>

{% if site.twitter_widget_id %}
<div class="text-tweets">
<div class="tweets">
<a class="twitter-timeline"
  data-dnt="true"
  width="600"
  height="250"
  href="https://twitter.com/{{ site.owner.twitter }}"
  data-widget-id="{{ site.twitter_widget_id }}"
  data-tweet-limit="2"
  data-chrome="noheader nofooter noborders noscrollbar transparent">
  Recent Tweets</a>
 </div>
<script>
    !function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+"://platform.twitter.com/widgets.js";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","twitter-wjs");
</script>
</div>
{% else %}
{% endif %}
