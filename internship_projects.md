---
layout: default
title: Internship Projects
permalink: /projects/internship/
---

# Internship Projects

These projects were completed during my professional internships, focusing on real-world challenges in cloud computing, DevOps, and software development.

[Back to Main Projects Page](../projects/)

---

<div class="project-list">
{% for project in site.projects %}
  {% if project.category == "Internship" %}
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