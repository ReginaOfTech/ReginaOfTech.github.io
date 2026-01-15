---
title: "Projects"
permalink: /projects/
classes: wide
---

A small set of projects that show how I build: clear problem framing, reliable implementation, and reviewer-friendly outputs.

{% if site.projects %}
  {% assign items = site.projects | sort: "order" %}

  <div class="project-list">
    {% for p in items %}
      <div class="project-item">
        <div class="project-title"><a href="{{ p.url | relative_url }}">{{ p.title }}</a></div>

        {% if p.one_liner %}
          <div class="project-subtitle">{{ p.one_liner }}</div>
        {% endif %}

        {% if p.tags %}
          <div class="project-tags">
            {% for t in p.tags %}
              <span class="tag-pill">{{ t }}</span>
            {% endfor %}
          </div>
        {% endif %}

        {% if p.highlights %}
          <ul class="project-bullets">
            {% for h in p.highlights %}
              <li>{{ h }}</li>
            {% endfor %}
          </ul>
        {% endif %}

        <div class="project-links">
          <a class="btn btn--inverse btn--small" href="{{ p.url | relative_url }}">Details</a>
          {% if p.repo_url %}
            <a class="btn btn--inverse btn--small" href="{{ p.repo_url }}" target="_blank" rel="noopener">GitHub</a>
          {% endif %}
        </div>
      </div>
    {% endfor %}
  </div>

{% else %}
_Projects collection is not enabled yet. Ensure `_config.yml` includes a `projects` collection and you have an `_projects/` folder._
{% endif %}
