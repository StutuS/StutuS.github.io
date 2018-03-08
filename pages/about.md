---
layout: page
title: About
description: 思考改变自己
keywords: Tao Zhang, 张涛
comments: true
menu: 关于
permalink: /about/
---

我是张涛，游走在思考的边缘。

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
