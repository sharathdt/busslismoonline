---
title: Authors
layout: page
permalink: /authors/
---

<div>
{% assign items_grouped = site.posts | group_by: 'author' %}
{% for group in items_grouped %}
<h3>{{group.name}}</h3>
{% for item in group.items %}
<li><a href="{{item.url}}">{{item.title}}</a></li>
{% endfor %}
{% endfor %}
</div>
