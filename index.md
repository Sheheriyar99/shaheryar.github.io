---
layout: default
title: Home
---

<!-- Hero Section -->
<section class="hero">
  <div class="container">
    <div class="hero-content">
      <h1>☁️ Cloud & AWS Engineering</h1>
      <p>Exploring cloud architecture, DevOps practices, and infrastructure as code</p>
      <div class="hero-buttons">
        <a href="https://aws.amazon.com/developer/community/builders/" class="cta-button" target="_blank">Apply for AWS Community Builder</a>
        <a href="#blog" class="cta-button secondary">Read My Blogs</a>
      </div>
    </div>
  </div>
</section>

<!-- About Section -->
<section class="about">
  <div class="container">
    <h2>Welcome to My Technical Journey</h2>
    <p>Hi! I'm <strong>Shaheryar Khalid</strong>, passionate about cloud computing, DevOps, and building scalable infrastructure. I share insights about AWS, Linux, Terraform, CDK, and real-world infrastructure challenges.</p>
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
    <h2>Ready to Apply for AWS Community Builder?</h2>
    <p>Join a global network of AWS experts and community leaders. Share your knowledge, grow your skills, and make an impact.</p>
    <a href="https://aws.amazon.com/developer/community/builders/" class="cta-button" target="_blank">Apply Now on AWS</a>
  </div>
</section>
