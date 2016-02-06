---
layout: page
title: All blog posts by topic or date
---
<h2>Posts by topic</h2>
<div>
  {% assign sorted_tags = site.data.tags | sort:"sort" %}<ul>
  {% for tag in sorted_tags %}
    <li> {% include tag_link_formatter.html tag=tag %}: {{ tag.title }}</li>
  {% endfor %}</ul>
</div><br>

<h2>Posts by date</h2>
<em>Note that some earlier posts have been retired; <a href="mailto:amandavisconti@gmail.com?Subject=ContactFromLiteratureGeekBlog">contact me</a> if you're having trouble finding something old, as I might have an offline copy to share.</em>
<section id="archive">
  <h3>This year's posts</h3>
  {%for post in site.posts %}
    {% unless post.next %}
      <ul class="this">
    {% else %}
      {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
      {% capture nyear %}{{ post.next.date | date: '%Y' }}{% endcapture %}
      {% if year != nyear %}
        </ul>
        <h3>{{ post.date | date: '%Y' }}</h3>
        <ul class="past">
      {% endif %}
    {% endunless %}
      <li><time>{{ post.date | date_to_string }}</time> <a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
  </ul>
</section>