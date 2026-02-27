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
social: false
---

<div class="post">
  <article>
    <!-- 1. Bio Section (Updated Wording) -->
    <div class="clearfix">
      <p>
        I am a Graduate Student at the <b>University of Macau</b>, majoring in Robotics and Autonomous Systems. <b>Currently, my work focuses on the intersection of Embodied AI and Task & Motion Planning (TAMP).</b>
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

    <!-- 2. Selected Works Section (Manual Layout for Precision) -->
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

      <!-- 1. V-LGP -->
      <div class="work-item">
        <div class="work-img">
          <img src="{{ 'assets/img/vlgp.gif' | relative_url }}" alt="V-LGP">
        </div>
        <div class="work-content">
          <div class="work-title">V-LGP: Vision-Language Geometric Programming for Long-Horizon Assembly</div>
          <div class="work-venue">Submitted to IEEE Robotics and Automation Letters (RA-L)</div>
          <div class="work-desc">
            A hierarchical framework bridging VLM reasoning with low-level LGP solvers. Enhanced the C++ KOMO solver with virtual anchors for multi-support consistency.
          </div>
          <div class="work-links">
            <a href="https://github.com/LeslieLinXinxiang/VLM-LGP" class="btn btn-outline-dark btn-sm" style="color: #333;">Code</a>
            <span class="btn btn-outline-secondary btn-sm disabled" style="color: #999;">PDF (Coming Soon)</span>
          </div>
        </div>
      </div>

      <!-- 2. Linkerbot -->
      <div class="work-item">
        <div class="work-img">
          <img src="{{ 'assets/img/vlm_agent.gif' | relative_url }}" alt="VLM Agent">
        </div>
        <div class="work-content">
          <div class="work-title">End-to-End Reasoning for Long-Horizon Autonomous Robotic Manipulation</div>
          <div class="work-venue">Collaboration with Linkerbot | Joint Lab Project</div>
          <div class="work-desc">
            Replaced traditional modular pipelines with vision-centric end-to-end intelligence on a 6-DOF JAKA Zu3 arm. Implemented a closed-loop reasoning agent using multimodal inputs to achieve autonomous decision-making and real-time game interaction with a dexterous hand.
          </div>
          <div class="work-links">
            <a href="https://github.com/LeslieLinXinxiang/VLM-Game-Agent" class="btn btn-outline-dark btn-sm" style="color: #333;">Code</a>
          </div>
        </div>
      </div>

      <!-- 3. Leaderdrive Humanoid -->
      <div class="work-item">
        <div class="work-img">
          <img src="{{ 'assets/img/collaboration_project.jpg' | relative_url }}" alt="Humanoid">
        </div>
        <div class="work-content">
          <div class="work-title">Mechatronic Design and Locomotion Deployment for Bipedal Humanoid</div>
          <div class="work-venue">Industry Collaboration with Leaderdrive</div>
          <div class="work-desc">
            Directed the structural design and integration of joint modules for a humanoid platform. Optimized locomotion stability by mitigating mechanical resonance and sensor noise during hardware-in-the-loop (HIL) testing and deployment.
          </div>
        </div>
      </div>

    </div>
  </article>
</div>
