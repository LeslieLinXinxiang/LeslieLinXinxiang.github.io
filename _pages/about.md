---
layout: about
title: about
permalink: /
subtitle: <a href='#'>Affiliations</a>. Address. Contacts. Motto. Etc.

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>555 your office number</p>
    <p>123 your address street</p>
    <p>Your City, State 12345</p>

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: true
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

<!-- ----------------------------------------------------------------------- -->
<!-- Selected Research & Highlights (首页精选项目) -->
<!-- ----------------------------------------------------------------------- -->

<div class="projects" style="margin-top: 50px;">
  <h2 style="border-bottom: 1px solid #eaecef; padding-bottom: 10px; font-weight: bold;">Selected Research & Projects</h2>

  <!-- 1. V-LGP Project -->
  <div class="row" style="margin-top: 30px; display: flex; align-items: flex-start;">
    <div class="col-sm-4" style="padding-right: 15px;">
      {% include figure.liquid path="assets/img/vlgp.gif" title="V-LGP" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-8">
      <h3 style="font-size: 1.2rem; font-weight: 700; margin-top: 0;">V-LGP: Vision-Language Geometric Programming</h3>
      <p style="font-size: 0.95rem; line-height: 1.5; text-align: justify;">
        A hierarchical framework bridging VLM reasoning with low-level LGP solvers for long-horizon robotic assembly. I specifically enhanced the <b>C++ KOMO solver</b> with <i>virtual anchors</i> to resolve multi-support physical constraints and implemented <i>geometric funnels</i> to ensure robust Sim-to-Real transfer.
      </p>
      <div class="links">
        <a href="https://github.com/LeslieLinXinxiang/VLM-LGP" class="btn btn-outline-dark btn-sm" style="padding: 2px 8px; font-size: 0.8rem;">Code</a>
        <span class="btn btn-outline-secondary btn-sm disabled" style="padding: 2px 8px; font-size: 0.8rem;">Paper (Under Review at RAL)</span>
      </div>
    </div>
  </div>

  <hr style="margin: 25px 0; border: 0; border-top: 1px solid #eee;">

  <!-- 2. VLM Agent Project -->
  <div class="row" style="display: flex; align-items: flex-start;">
    <div class="col-sm-4" style="padding-right: 15px;">
      {% include figure.liquid path="assets/img/vlm_agent.gif" title="VLM Agent" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-8">
      <h3 style="font-size: 1.2rem; font-weight: 700; margin-top: 0;">Multimodal Reasoning for Dexterous Manipulation</h3>
      <p style="font-size: 0.95rem; line-height: 1.5; text-align: justify;">
        Integrated an end-to-end VLM agent with <b>Lingxin Dexterous Hands</b>. This work focuses on grounding vision-language instructions into high-precision tactile and grasp planning. Successfully resolved contact-stability issues during real-world logic execution through refined motor torque profiles.
      </p>
      <div class="links">
        <a href="https://github.com/LeslieLinXinxiang/VLM-Game-Agent" class="btn btn-outline-dark btn-sm" style="padding: 2px 8px; font-size: 0.8rem;">Code</a>
      </div>
    </div>
  </div>

  <hr style="margin: 25px 0; border: 0; border-top: 1px solid #eee;">

  <!-- 3. Humanoid Project -->
  <div class="row" style="display: flex; align-items: flex-start;">
    <div class="col-sm-4" style="padding-right: 15px;">
      {% include figure.liquid path="assets/img/collaboration_project.jpg" title="Humanoid Integration" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-8">
      <h3 style="font-size: 1.2rem; font-weight: 700; margin-top: 0;">Mechatronic Design for Bipedal Humanoid Platforms</h3>
      <p style="font-size: 0.95rem; line-height: 1.5; text-align: justify;">
        <b>Industry Collaboration with Greenland Harmonic.</b> Focused on the development and system-wide integration of high-torque density joint modules. Conducted <i>Hardware-in-the-Loop (HIL)</i> testing and vibration analysis to eliminate mechanical resonance for stable locomotion.
      </p>
    </div>
  </div>
</div>
