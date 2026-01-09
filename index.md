---
layout: default
title: Home
---

<!-- Hero Section -->
<section class="hero">
  <div class="container">
    <div class="hero-content">
      <h1>☁️ AWS Services & Cloud Engineering</h1>
      <p>In-depth guides, tutorials, and best practices for AWS services</p>
      <div class="hero-buttons">
        <a href="#blog" class="cta-button">Explore Articles</a>
      </div>
    </div>
  </div>
</section>

<!-- About Section -->
<section class="about">
  <div class="container">
    <h2>Master AWS Services</h2>
    <p>Comprehensive tutorials and best practices for AWS services. Learn EC2, Lambda, S3, RDS, CloudFormation, CDK, and more. Explore cloud architecture, DevOps practices, and infrastructure automation.</p>
  </div>
</section>

<!-- Latest Blog Posts -->
<section class="blog-section" id="blog">
  <div class="container">
    <h2>Latest Blog Posts</h2>
    <div class="blog-grid">
      {% for post in site.posts limit:6 %}
      <article class="blog-card">
        <div class="blog-date">{{ post.date | date: "%B %d, %Y" }}</div>
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <p>{{ post.excerpt | strip_html | truncatewords: 20 }}</p>
        <a href="{{ post.url }}" class="read-more">Read More →</a>
      </article>
      {% endfor %}
    </div>
    {% if site.posts.size > 6 %}
    <div class="view-all">
      <a href="/blog" class="cta-button">View All Posts</a>
    </div>
    {% endif %}
  </div>
</section>

<!-- CTA Section -->
<section class="cta-section">
  <div class="container">
    <h2>Start Learning AWS Today</h2>
    <p>Explore practical guides and tutorials for AWS services and cloud best practices.</p>
    <a href="/blog" class="cta-button">View All Articles</a>
  </div>
</section>
