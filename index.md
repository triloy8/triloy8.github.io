---
layout: default
title: Home
---

# Posts

<ul class="posts">
{%- for post in site.posts -%}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="muted">— {{ post.date | date: "%b %-d, %Y" }}</span>
  </li>
{%- endfor -%}
</ul>

<p class="muted">Subscribe via <a href="{{ '/feed.xml' | relative_url }}">RSS</a>.</p>