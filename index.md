---
layout: single
title: "Regina Baker"
permalink: /
author_profile: false
classes: wide
---

<div class="hero-block">
  <div class="hero-kicker">Software Engineer</div>
  <h1 class="hero-title">
    Building reliable, production-ready AI systems<br/>
    for high-stakes environments.
  </h1>

  <div class="hero-actions">
    <a class="btn btn--primary" href="/projects/">View Projects</a>
    <a class="btn btn--inverse" href="https://github.com/ReginaOfTech" target="_blank" rel="noopener">GitHub</a>
  </div>
</div>

<hr class="section-rule" />

## What I do

<div class="grid-2">
  <div class="card">
    <div class="card-title">Reliable AI systems</div>
    <div class="card-body">
      I build AI-enabled software that prioritizes correctness, testability, and operational clarity.
    </div>
  </div>

  <div class="card">
    <div class="card-title">Production-first engineering</div>
    <div class="card-body">
      I focus on maintainable pipelines, measurable outcomes, and pragmatic tradeoffs—without hype.
    </div>
  </div>
</div>

<hr class="section-rule" />

## Selected projects

<div class="project-list">
  {% assign featured_items = site.projects | where: "featured", true | sort: "order" %}

  {% for p in featured_items limit:3 %}
    <div class="project-item">
      <div class="project-title"><a href="{{ p.url | relative_url }}">{{ p.title }}</a></div>

      {% if p.one_liner %}
        <div class="project-subtitle">{{ p.one_liner }}</div>
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

  {% if featured_items.size == 0 %}
    <div class="card">
      <div class="card-title">Projects coming soon</div>
      <div class="card-body">Featured work will appear here as it’s added.</div>
    </div>
  {% endif %}
</div>


<hr class="section-rule" />

## Skills Stack

<div class="cred-strip">
  <div><span class="cred-label">Focus:</span> Reliable AI-enabled systems • production quality • auditability</div>
  <div><span class="cred-label">Security:</span> Secure design • validation • testability</div>
    <div><span class="cred-label">Tools:</span> Python • C++ • Linux • CI/CD</div>
    <div><span class="cred-label">Credentials:</span> Security+ • AWS Cloud Practitioner</div>
    <div><span class="cred-label">Leadership:</span> Test Lead • AI Roundtable Lead (DCS Corporation)</div>
</div>


<hr class="section-rule" />

<div class="cta-bar">
  <div class="cta-text">
    If you’re hiring for reliable, production-first AI systems work, I can be found on LinkedIn.
  </div>
  <div class="cta-actions">
    <a class="btn btn--inverse" href="/about/">About</a>
  </div>
</div>
