---
layout: page
permalink: /projects/
title: projects
nav: true
nav_order: 3
---

<div class="projects" style="margin-top: 30px;">
  {% for item in site.data.works %}
    {% if item.type == 'project' %}
      <div class="row mb-5" style="display: flex; gap: 20px; align-items: flex-start;">
        <div class="col-sm-4"><img src="{{ item.img | relative_url }}" class="img-fluid rounded border"></div>
        <div class="col-sm-8">
          <h4 style="font-size: 1.05rem; font-weight: 600;">{{ item.title }}</h4>
          <p style="font-size: 0.85rem; line-height: 1.4; color: #444; margin-top: 8px;">{{ item.desc }}</p>
          {% if item.code %}<a href="{{ item.code }}" class="btn btn-outline-dark btn-sm mt-2">Code</a>{% endif %}
        </div>
      </div>
    {% endif %}
  {% endfor %}
</div>
