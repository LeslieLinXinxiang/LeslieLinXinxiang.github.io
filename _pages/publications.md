---
layout: page
permalink: /publications/
title: publications
nav: true
nav_order: 3
---

<!-- _pages/publications.md -->
<div class="publications" style="margin-top: 30px;">
  <h2 style="font-size: 1.25rem; font-weight: 700; margin-bottom: 25px; border-bottom: 1px solid #eee; padding-bottom: 10px;">Preprints & Under Review</h2>

  {% for item in site.data.works %}
    {% if item.type == 'publication' %}
      <div class="row" style="display: flex; gap: 20px; align-items: flex-start; margin-bottom: 40px;">
        <!-- 图片区域 -->
        <div class="col-sm-4">
          <img src="{{ item.img | relative_url }}" class="img-fluid rounded border" alt="{{ item.title }}">
        </div>
        
        <!-- 内容区域 -->
        <div class="col-sm-8">
          <h4 style="font-size: 1.05rem; font-weight: 600; margin-bottom: 5px; color: #333;">{{ item.title }}</h4>
          <p style="font-size: 0.9rem; margin-bottom: 5px;">{{ item.authors }}</p>
          <p style="font-size: 0.9rem; color: #666; font-style: italic; margin-bottom: 8px;">{{ item.venue }}</p>
          <p style="font-size: 0.88rem; line-height: 1.45; color: #444; text-align: justify;">{{ item.desc }}</p>
          
          <div style="margin-top: 12px;">
            {% if item.code %}
              <a href="{{ item.code }}" class="btn btn-outline-dark btn-sm" style="font-size: 0.75rem; padding: 2px 10px;">Code</a>
            {% endif %}
            {% if item.pdf == "" or item.pdf == nil %}
              <a class="btn btn-outline-secondary btn-sm disabled" style="font-size: 0.75rem; padding: 2px 10px; color: #999;">PDF (Coming Soon)</a>
            {% else %}
              <a href="{{ item.pdf | relative_url }}" class="btn btn-outline-dark btn-sm" style="font-size: 0.75rem; padding: 2px 10px;">PDF</a>
            {% endif %}
          </div>
        </div>
      </div>
    {% endif %}
  {% endfor %}
</div>
