---
title: "Projects"
permalink: /projects/
classes: wide
---

A small set of projects that show how I build: clear problem framing, reliable implementation, and reviewer-friendly outputs.

{% if site.projects %}
  {% assign items = site.projects | sort: "order" %}

  {% if items.size > 0 %}
    {% for p in items %}
### [{{ p.title }}]({{ p.url }})
{{ p.one_liner }}
    {% endfor %}
  {% else %}
_No projects have been added yet. Check back soon._
  {% endif %}

{% else %}
_Projects collection is not enabled yet. Ensure `_config.yml` includes a `projects` collection and you have an `_projects/` folder._
{% endif %}
