---
layout: default
title: Blog
permalink: /blog/
---

<div class="blog-page">
  <div class="container">
    <h1>All Blog Posts</h1>
    
    <div class="blog-list">
      {% for post in site.posts %}
      <article class="blog-list-item">
        <div class="blog-meta">
          <span class="date">{{ post.date | date: "%B %d, %Y" }}</span>
          {% if post.categories %}
          <div class="categories">
            {% for category in post.categories %}
            <span class="category">{{ category }}</span>
            {% endfor %}
          </div>
          {% endif %}
        </div>
        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
        <p class="excerpt">{{ post.excerpt | strip_html }}</p>
        <a href="{{ post.url }}" class="read-more">Read Article →</a>
      </article>
      {% endfor %}
    </div>
  </div>
</div>
