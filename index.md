---
layout: default
title: 我思故我在
---

## {{ page.title }}

#### 文章列表：
{% for post in site.posts %}

  <li>
    {{ post.date | date_to_string }} <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
  </li>

{% endfor %}

#### [jekyll 帮助](https://jekyllrb.com/docs/pages/)

#### 测试区域

<div>
    <h1>What are in this site?</h1>
    {% for item in site %}
      <li>
        <a>{{ item } </a>
      </li>
    {% endfor %}
</div>