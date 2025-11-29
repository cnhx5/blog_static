---
layout: home
title: Home
permalink: /
---

# Welcome to My Blog! 🚀
I write about coding, tech tips, and personal projects. Browse my posts below:

{% raw %}{% for post in site.posts %}
  <div class="post-card">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt | strip_html | truncate: 150 }}</p>
    <a href="{{ post.url | relative_url }}">Read more →</a>
  </div>
{% endfor %}{% endraw %}

If no posts are shown yet, I'm still working on my first article!
