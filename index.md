---
layout: default
title: 我的Blog
---

{{ page.title }}

#### md首页

{% for post in site.posts %}

  <li>{{ post.date | date_to_string }} <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>

{% endfor %}


#### Liquid Filters

Absolute URL

```html
{{ "/assets/style.css" | absolute_url }}
```
{{ "/assets/style.css" | absolute_url }}

```html
{{ site }}
```
{{ site }}

```html
{{ site.members }}
```
{{ site.members }}


```html
{{ site | jsonify }}
```
{{ site | jsonify }}



