---
title: "Projects"
permalink: /projects/
layout: collection
collection: projects
entries_layout: grid
classes: wide
---

{% for project in site.projects %}
  <div class="project-tile">
    <h2>{{ project.title }}</h2>
    <img src="{{ project.image | relative_url }}" alt="{{ project.title }}">
    <p>{{ project.excerpt }}</p>
    <h3>Skills Gained:</h3>
    <ul>
      {% for skill in project.skills %}
        <li>{{ skill }}</li>
      {% endfor %}
    </ul>
  </div>
{% endfor %}