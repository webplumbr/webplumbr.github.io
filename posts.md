---
layout: list_of_posts
title: Blog posts
---
<h1>Latest Posts</h1>

<ul>
  {% for post in site.posts %}
    <li class="link-to-post">
      <h3 class="post-date">{{ post.date | date: '%B %e, %Y' }}</h3>
      <p>{{ post.excerpt }}</p>
      <p class="read-more"><a href="{{ post.url }}">To continue reading...</a></p>
    </li>
  {% endfor %}
</ul>