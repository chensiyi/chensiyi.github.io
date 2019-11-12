---
layout: default
title: 我思故我在
---

## {{ page.title }}

#### 文章列表：
{% for post in paginator.posts %}

  <li>
    {{ post.date | date_to_string }} <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
  </li>

{% endfor %}

<div class="pagination">
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path }}" class="previous">
      Previous
    </a>
  {% else %}
    <span class="previous">Previous</span>
  {% endif %}
  <span class="page_number ">
    Page: {{ paginator.page }} of {{ paginator.total_pages }}
  </span>
  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path }}" class="next">Next</a>
  {% else %}
    <span class="next ">Next</span>
  {% endif %}
</div>


[jekyll 帮助](https://jekyllrb.com/docs/pages/)

