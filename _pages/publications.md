---
layout: page
permalink: /publications/
title: publications
nav: true
nav_order: 3
---

<!-- =====================================================================
     CUSTOM CSS FOR UNIFORM BUTTONS
     ===================================================================== -->
<style>
  /* 1. Code 按钮：黑边白底 */
  .btn-code { 
    font-size: 0.75rem; padding: 2px 8px; border: 1px solid #333; border-radius: 3px; 
    color: #333; background-color: #fff; text-decoration: none; margin-right: 5px; 
    display: inline-block; 
  }
  .btn-code:hover { background-color: #333; color: #fff; text-decoration: none; }

  /* 2. PDF 按钮：红边白底 */
  .btn-pdf-soon { 
    font-size: 0.75rem; padding: 2px 8px; border: 1px solid #d32f2f; border-radius: 3px; 
    color: #d32f2f; background-color: #fff; text-decoration: none; margin-right: 5px; 
    display: inline-block; cursor: not-allowed; opacity: 0.8; 
  }

  /* 图片统一尺寸 (180px 高度) */
  .pub-img-box {
    height: 180px; width: 100%; display: flex; align-items: center; justify-content: center;
    background-color: #fcfcfc; border: 1px solid #f0f0f0; border-radius: 5px;
  }
  .pub-img-box img { max-height: 100%; max-width: 100%; object-fit: contain; }
</style>

<div class="publications" style="margin-top: 30px;">
  <h2 style="font-size: 1.25rem; font-weight: 700; margin-bottom: 25px; border-bottom: 1px solid #eee; padding-bottom: 10px;">Preprints & Under Review</h2>

  {% for item in site.data.works %}
    {% if item.type == 'publication' %}
      <div class="row" style="display: flex; gap: 20px; align-items: flex-start; margin-bottom: 40px;">
        <!-- 图片区域 -->
        <div class="col-sm-4">
          <div class="pub-img-box">
            <img src="{{ item.img | relative_url }}" alt="{{ item.title }}">
          </div>
        </div>
        
        <!-- 内容区域 -->
        <div class="col-sm-8">
          <h4 style="font-size: 1.05rem; font-weight: 600; margin-bottom: 5px; color: #333;">{{ item.title }}</h4>
          <p style="font-size: 0.9rem; margin-bottom: 5px;">{{ item.authors }}</p>
          <p style="font-size: 0.9rem; color: #666; font-style: italic; margin-bottom: 8px;">{{ item.venue }}</p>
          <p style="font-size: 0.88rem; line-height: 1.45; color: #444; text-align: justify;">{{ item.desc }}</p>
          
          <div class="work-links" style="margin-top: 12px;">
            {% if item.code %}
              <a href="{{ item.code }}" class="btn-code">Code</a>
            {% endif %}
            
            {% if item.pdf == "" or item.pdf == nil %}
              <span class="btn-pdf-soon">PDF (Coming Soon)</span>
            {% else %}
              <a href="{{ item.pdf | relative_url }}" class="btn-code">PDF</a>
            {% endif %}
          </div>
        </div>
      </div>
    {% endif %}
  {% endfor %}
</div>
