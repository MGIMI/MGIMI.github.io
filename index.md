---
layout: default
---

# Institute Blog

<dl>
  {% for post in site.posts limit:7 %}
    <dt>{{ post.date　| date: "%Y年%m月%d日" }}</dt>
    <dd>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </dd>
  {% endfor %}
</dl>

[[more...]]({{ site.url }}/index_all.html)
