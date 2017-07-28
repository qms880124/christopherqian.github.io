---
layout: page
title: About
description: 一身转战三千里，一剑曾当百万师
keywords: Christopher Qian
comments: true
menu: 关于
permalink: /about/
---

不念过去，不畏将来。

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
