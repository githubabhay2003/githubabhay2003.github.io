---
layout: default
title: My Blog
permalink: /blog/
---

# My Blog

A collection of my articles on cloud computing, DevOps, and automation, originally published on Medium.

[Back to Home](./index.md)

---

<div class="post-list">
  {% for post in site.posts %}
    <article class="post-item" style="margin-bottom: 2.5em;">
      <h2 style="margin-bottom: 0.2em;">
        <a href="{{ post.medium_link }}" target="_blank" rel="noopener noreferrer" style="text-decoration: none; color: inherit;">
          {{ post.title }}
        </a>
      </h2>
      <p class="post-meta" style="color: #666; font-size: 0.9em;">
        Published on {{ post.date | date: "%B %-d, %Y" }}
      </p>
      <p>{{ post.summary }}</p>
      <p>
        <a href="{{ post.medium_link }}" target="_blank" rel="noopener noreferrer">
          Read the full article on Medium →
        </a>
      </p>
    </article>
  {% endfor %}
</div>