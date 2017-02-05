---
layout: page
title: Blog of Marko
tagline: under construction
---
{% include JB/setup %}
    
## My Posts

This blog is under construction - notably the layout ;-)

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>


