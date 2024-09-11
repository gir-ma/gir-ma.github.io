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
    {% if project.header.teaser %}
      <img src="{{ project.header.teaser | relative_url }}" alt="{{ project.title }}">
    {% endif %}
    <p>{{ project.excerpt }}</p>
    {% if project.skills %}
      <h3>Skills:</h3>
      <ul>
        {% for skill in project.skills %}
          <li>{{ skill }}</li>
        {% endfor %}
      </ul>
    {% endif %}
    <a href="{{ project.url | relative_url }}" class="btn btn--primary">Read More</a>
  </div>
{% endfor %}