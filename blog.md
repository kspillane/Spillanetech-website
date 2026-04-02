---
layout: default
title: Blog
---

<section class="section" style="padding-top: calc(var(--header-height) + 2rem);">
  <div class="container">
    <div class="section-title">
      <h1>Insights</h1>
      <p class="lead" style="margin-top: 1rem; color: var(--color-text-muted);">Thoughts and opinions on technology, cybersecurity, and business.</p>
    </div>
    
    <div class="grid grid-3">
      {% for post in site.posts %}
        <div class="pillar-card" style="text-align: left;">
          <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
          <p class="text-muted">{{ post.date | date: "%b %-d, %Y" }}</p>
          <p>{{ post.description }}</p>
          <a href="{{ post.url | relative_url }}" class="text-accent">Read More →</a>
        </div>
      {% endfor %}
    </div>
  </div>
</section>
