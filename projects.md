---
layout: default
title: My Projects
permalink: /projects/
---

# My Projects

My work is divided into two categories. Please select one to view the relevant projects.

---

<style>
  .category-card {
    border: 1px solid #ddd;
    padding: 1.5em;
    margin-bottom: 1.5em;
    border-radius: 8px;
    transition: all 0.2s ease-in-out;
    cursor: pointer;
  }
  .category-card:hover {
    border-color: #007bff;
    transform: translateY(-5px);
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  }
  .category-card h2 {
    margin-top: 0;
  }
  .category-card h2 a {
    text-decoration: none;
    color: inherit;
  }
  .category-card h2 a:hover {
    text-decoration: underline;
  }
</style>

<div class="category-card" onclick="window.location.href='/projects/internship/'">
  <h2><a href="/projects/internship/">📁 Internship Projects</a></h2>
  <p>Projects completed during my professional internships, focusing on real-world DevOps and cloud challenges.</p>
</div>

<div class="category-card" onclick="window.location.href='/projects/personal/'">
  <h2><a href="/projects/personal/">👤 Personal Projects</a></h2>
  <p>A collection of my self-driven projects, exploring various technologies in AI, automation, and system administration.</p>
</div>