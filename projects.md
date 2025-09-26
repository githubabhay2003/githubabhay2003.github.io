---
layout: default
title: My Projects
permalink: /projects/
---

# My Projects

A collection of my professional and personal work, demonstrating my skills in cloud engineering, DevOps, and automation.

---

## Internship Projects

<div class="project-list">
{% for project in site.projects %}
  {% if project.category == "Internship" %}
    <div class="project-item">
      <h3>{{ project.title }}</h3>
      <p><em><strong>Tech Stack:</strong> {{ project.tech-stack }}</em></p>
      {{ project.content | strip_html | truncatewords: 50 }}
      <p class="project-links">
        {% if project.github-link %}<a href="{{ project.github-link }}" target="_blank" rel="noopener noreferrer">View on GitHub</a>{% endif %}
        {% if project.live-demo %}<a href="{{ project.live-demo }}" target="_blank" rel="noopener noreferrer">Live Demo</a>{% endif %}
      </p>
    </div>
  {% endif %}
{% endfor %}
</div>

---

## Personal Projects

<div class="project-list">
{% for project in site.projects %}
  {% if project.category == "Personal" %}
    <div class="project-item">
      <h3>{{ project.title }}</h3>
      <p><em><strong>Tech Stack:</strong> {{ project.tech-stack }}</em></p>
      {{ project.content | strip_html | truncatewords: 50 }}
      <p class="project-links">
        {% if project.github-link %}<a href="{{ project.github-link }}" target="_blank" rel="noopener noreferrer">View on GitHub</a>{% endif %}
        {% if project.live-demo %}<a href="{{ project.live-demo }}" target="_blank" rel="noopener noreferrer">Live Demo</a>{% endif %}
      </p>
    </div>
  {% endif %}
{% endfor %}
</div>
