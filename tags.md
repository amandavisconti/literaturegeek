---
layout: page
title: View posts by topic
---
<div class="page">
  {% assign sorted_tags = site.data.tags | sort:"sort" %}<ul>
  {% for tag in sorted_tags %}
    <li> {% include tag_link_formatter.html tag=tag %}: {{ tag.title }}</li>
  {% endfor %}</ul>
</div>
