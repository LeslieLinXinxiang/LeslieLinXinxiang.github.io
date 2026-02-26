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

<div class="projects">
  <h2 style="margin-top: 40px; border-bottom: 1px solid #eaecef; padding-bottom: 10px; font-weight: bold;">Selected Research & Projects</h2>

  <!-- 项目 1: V-LGP -->
  <div class="row" style="margin-top: 30px; display: flex; align-items: flex-start;">
    <div class="col-sm-5" style="padding-right: 20px;">
      {% include figure.liquid path="assets/img/vlgp.gif" title="V-LGP" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-7">
      <h3 style="font-size: 1.25rem; font-weight: 700; margin-top: 0;">V-LGP: Vision-Language Geometric Programming</h3>
      <p style="font-size: 0.95rem; line-height: 1.5; text-align: justify;">
        We developed a hierarchical framework that bridges high-level semantic reasoning with low-level geometric optimization for long-horizon robotic assembly. By leveraging VLMs as task pruners, we reduced the logic search space significantly. I specifically enhanced the <b>C++ KOMO solver</b> with <i>virtual anchors</i> to resolve multi-support physical constraints and implemented <i>geometric funnels</i> to ensure robust Sim-to-Real transfer.
      </p>
      <div class="links">
        <a href="https://github.com/LeslieLinXinxiang/VLM-LGP" class="btn btn-outline-dark btn-sm" style="padding: 2px 8px;">Code</a>
        <span class="btn btn-outline-secondary btn-sm disabled" style="padding: 2px 8px;">Paper (Under Review at RAL)</span>
      </div>
    </div>
  </div>

  <hr style="margin: 30px 0; border: 0; border-top: 1px solid #eee;">

  <!-- 项目 2: VLM Agent -->
  <div class="row" style="display: flex; align-items: flex-start;">
    <div class="col-sm-5" style="padding-right: 20px;">
      {% include figure.liquid path="assets/img/vlm_agent.gif" title="VLM Agent" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-7">
      <h3 style="font-size: 1.25rem; font-weight: 700; margin-top: 0;">Multimodal Reasoning for Dexterous Manipulation</h3>
      <p style="font-size: 0.95rem; line-height: 1.5; text-align: justify;">
        Deployed an end-to-end multimodal agent on a dual-arm robot platform integrated with <b>Lingxin Dexterous Hands</b>. The project focused on grounding vision-language instructions into high-precision tactile and grasp planning. I resolved contact-stability issues during real-world Tic-Tac-Toe game execution through refined motor torque profiles and contact priors.
      </p>
      <div class="links">
        <a href="https://github.com/LeslieLinXinxiang/VLM-Game-Agent" class="btn btn-outline-dark btn-sm" style="padding: 2px 8px;">Code</a>
      </div>
    </div>
  </div>

  <hr style="margin: 30px 0; border: 0; border-top: 1px solid #eee;">

  <!-- 项目 3: Humanoid -->
  <div class="row" style="display: flex; align-items: flex-start;">
    <div class="col-sm-5" style="padding-right: 20px;">
      {% include figure.liquid path="assets/img/collaboration_project.jpg" title="Humanoid Integration" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-7">
      <h3 style="font-size: 1.25rem; font-weight: 700; margin-top: 0;">Mechatronic Design for Bipedal Humanoid Platforms</h3>
      <p style="font-size: 0.95rem; line-height: 1.5; text-align: justify;">
        <b>Industry Collaboration with Greenland Harmonic.</b> Focused on the development and system-wide integration of high-torque density joint modules. I conducted <i>Hardware-in-the-Loop (HIL)</i> testing and vibration analysis to eliminate mechanical resonance, enabling more stable locomotion control on bipedal hardware.
      </p>
      <div class="badge badge-secondary" style="font-weight: 400;">Full-stack Mechatronics</div>
    </div>
  </div>
</div>
