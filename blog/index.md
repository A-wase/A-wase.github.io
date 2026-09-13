---
layout: default
title: Blog
---

# Blog

{% for post in site.posts %}
  <article>
    <h2>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h2>

    <p class="post-date">
      {{ post.date | date: "%d %B %Y" }}
    </p>

    {{ post.excerpt }}
  </article>
{% else %}
  <p>No posts yet.</p>
{% endfor %}