---
layout: page
title: Posts
permalink: /posts/
---

<div class="posts">
  {% for post in site.posts %}
    <article class="post">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
      <p>{{ post.excerpt }}</p>
    </article>
  {% endfor %}
</div>
