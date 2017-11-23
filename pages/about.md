---
layout: page
title: 关于我
description: 对于我的介绍
keywords: Jackeyzheng, 郑起
comments: true
menu: 关于
permalink: /about
---

我是郑起，一名程序员，为了自己微小而美好的愿景而努力。

曾就职于大街网和腾讯，目前在支付宝担任技术专家

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## 关注技术

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
