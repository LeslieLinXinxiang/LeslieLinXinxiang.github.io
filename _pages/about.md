---
layout: about
title: about
permalink: /
subtitle: Graduate Student @ <a href="https://www.um.edu.mo/">University of Macau</a> | Robotics & Autonomous Systems

profile:
  align: right
  image: selfie.jpg
  image_circular: false

news: false
selected_papers: false
social: true
---

<div class="post">
  <article>
    <!-- 1. Bio Section -->
    <div class="clearfix">
      <p>
        I am a Graduate Student at the <b>University of Macau</b>, majoring in Robotics and Autonomous Systems. My research interests lie at the intersection of <b>Embodied AI</b> and <b>TAMP (Task and Motion Planning)</b>.
      </p>
      <p>
        Specifically, I am exploring how Vision-Language Models (VLMs) can be integrated with geometric solvers to achieve long-horizon manipulation in real-world environments. I am passionate about bridging the gap between high-level reasoning and low-level physical execution.
      </p>
      <p>
        Before my graduate studies, I spent three years in the robotics and smart hardware industry, contributing to the mass production of several consumer-grade robots and products.
      </p>
      <p>
        If you have any questions or would like to discuss potential collaborations, feel free to reach out via <a href="mailto:Leslie.Linxinxiang@connect.um.edu.mo">email</a>.
      </p>
    </div>

    <!-- 2. Selected Works Section (Data-Driven) -->
    <div class="selected-works" style="margin-top: 50px;">
      <h2 style="font-size: 1.5rem; border-bottom: 1.5px solid #333; padding-bottom: 8px; margin-bottom: 25px;">Selected Works</h2>
      
      <style>
        .work-item { display: flex; align-items: flex-start; margin-bottom: 35px; gap: 20px; }
        .work-img { flex: 0 0 220px; max-width: 220px; }
        .work-img img { width: 100%; height: 130px; object-fit: cover; border-radius: 4px; border: 1px solid #f0f0f0; }
        .work-content { flex: 1; }
        .work-title { font-size: 1.05rem; font-weight: 600; margin: 0 0 5px 0; color: #333; }
        .work-venue { font-size: 0.85rem; color: #777; margin-bottom: 8px; font-style: italic; }
        .work-desc { font-size: 0.88rem; line-height: 1.45; color: #444; text-align: justify; }
        .work-links { margin-top: 8px; }
        .work-links a { font-size: 0.75rem; padding: 1px 8px; border: 1px solid #ccc; border-radius: 3px; color: #555; text-decoration: none; margin-right: 5px; }
        .work-links a:hover { background: #f8f8f8; border-color: #999; }
      </style>

      {% for item in site.data.works %}
        <div class="work-item">
          <div class="work-img">
            <img src="{{ item.img | relative_url }}" alt="{{ item.title }}">
          </div>
          <div class="work-content">
            <div class="work-title">{{ item.title }}</div>
            <div class="work-venue">{{ item.venue }}</div>
            <div class="work-desc">{{ item.desc }}</div>
            <div class="work-links">
              {% if item.code %}
                <a href="{{ item.code }}" class="btn btn-outline-dark btn-sm">Code</a>
              {% endif %}
              {% if item.type == 'publication' %}
                <a class="btn btn-outline-secondary btn-sm disabled" style="color: #999;">PDF (Coming Soon)</a>
              {% endif %}
            </div>
          </div>
        </div>
      {% endfor %}
    </div> <!-- End selected-works -->

  </article>
</div> <!-- End post -->
