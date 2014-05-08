---
layout: page
title: Summer of Wearables
tagline: Developing for small hardware
---
{% include JB/setup %}

{% assign post = site.posts.first %}
{% assign content = post.content %}
{% include post_details.html %}

## More

<ul class="posts">
  {% for p in site.posts %}
    {% if p.url != post.url %}
      <li><span>{{ p.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ p.url }}">{{ p.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>


