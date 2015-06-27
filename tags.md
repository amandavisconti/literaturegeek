---
layout: page
title: View posts by topic
---
<div class="page">
  {% assign sorted_tags = site.data.tags | sort:"sort" %}
  {% for tag in sorted_tags %}
    {% include tag_link_formatter.html tag=tag tag_separator='<br />' %}
  {% endfor %}
</div>
