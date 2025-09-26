---
layout: default
title: Personal Projects
permalink: /projects/personal/
---

# Personal Projects

This is a collection of my self-driven projects, created to explore new technologies and solve interesting problems in AI, automation, and system administration.

[Back to Main Projects Page](../projects/)

---

<div class="project-list">
{% for project in site.projects %}
  {% if project.category == "Personal" %}
    <div class="project-item">
      <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
      <p><em><strong>Tech Stack:</strong> {{ project.tech-stack }}</em></p>
      <p>{{ project.summary }}</p> {# <--- THIS IS THE FIX #}
      <p class="project-links">
        <a href="{{ project.url | relative_url }}">Read More...</a>
        {% if project.github-link %}| <a href="{{ project.github-link }}" target="_blank" rel="noopener noreferrer">View on GitHub</a>{% endif %}
      </p>
    </div>
  {% endif %}
{% endfor %}
</div>