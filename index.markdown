---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
# layout: default
title: My Blog
---

# Welcome to My Blog

This is where I share my thoughts, projects, and discoveries. Feel free to explore my recent posts below.

## Recent Posts

{% raw %}
{% for post in site.posts %}
  <div class="post-preview">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt }}</p>
    <a href="{{ post.url | relative_url }}">Read more...</a>
  </div>
  <hr>
{% endfor %}
{% endraw %}
