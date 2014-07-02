---
title: Blog
layout: default
---

<table class="table">
{% for post in site.posts %}
    {% if post.layout == 'post' %}
    <tr>
      <td>{{ post.date | date_to_long_string }}</td>
      <td><a href="{{ post.url }}">{{ post.title }}</a></td>
    </tr>
    {% endif %}
{% endfor %}
</table>
