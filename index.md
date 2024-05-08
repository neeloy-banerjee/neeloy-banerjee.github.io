---
layout: default
title: Home
---

<div class="main-content">
  <div class="posts">
    <h1 class="page-heading">Posts</h1>
    <ul class="post-list">
      {% for post in site.posts %}
        <li class="post-item">
          <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
          <h2 class="post-title">
            <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
          </h2>
        </li>
      {% endfor %}
    </ul>
  </div>
  <div class="sidebar">
    <h2>About</h2>
    <p>{{ site.description }}</p>
  </div>
</div>

<p class="rss-subscribe">Subscribe <a href="{{ '/feed.xml' | relative_url }}">via RSS</a></p>

