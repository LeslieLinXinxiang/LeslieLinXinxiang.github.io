---
layout: about
title: about
permalink: /
subtitle: Graduate Student @ <a href="https://www.um.edu.mo/">University of Macau</a> | Robotics & Autonomous Systems

profile:
  align: right
  image: selfie.jpg  # 已经按你的要求修改为 selfie.jpg
  image_circular: false
  more_info: >
    <p>Macau, China</p>

news: false
selected_papers: false
social: true
---

<div class="post">
  <article>
    <div class="clearfix">
      <p>
        I am a Graduate Student at the <b>University of Macau</b>, majoring in Robotics and Autonomous Systems. My research interests lie at the intersection of <b>Embodied AI</b> and <b>TAMP (Task and Motion Planning)</b>.
      </p>
      <p>
        Specifically, I am exploring how Vision-Language Models (VLMs) can be integrated with geometric solvers to achieve long-horizon manipulation in real-world environments. I am passionate about bridging the gap between high-level reasoning and low-level physical execution.
      </p>
      <p>
        If you have any questions or would like to discuss potential collaborations, feel free to reach out via <a href="mailto:Leslie.Linxinxiang@connect.um.edu.mo">email</a>.
      </p>
    </div>

    <!-- 精选项目 (Selected Research & Projects) -->
    <div class="selected-works" style="margin-top: 50px;">
      <h2 style="font-size: 1.5rem; border-bottom: 1px solid #333; padding-bottom: 8px; margin-bottom: 25px;">Selected Works</h2>

      <style>
        .work-item { display: flex; align-items: flex-start; margin-bottom: 30px; gap: 20px; }
        .work-img { flex: 0 0 200px; max-width: 200px; }
        .work-img img { width: 100%; height: 120px; object-fit: cover; border-radius: 4px; border: 1px solid #eee; }
        .work-content { flex: 1; }
        .work-title { font-size: 1.05rem; font-weight: 600; margin: 0 0 5px 0; color: #333; }
        .work-venue { font-size: 0.85rem; color: #777; margin-bottom: 8px; font-style: italic; }
        .work-desc { font-size: 0.88rem; line-height: 1.4; color: #444; text-align: justify; }
        .work-links { margin-top: 8px; }
        .work-links a { font-size: 0.75rem; padding: 1px 8px; border: 1px solid #ccc; border-radius: 3px; color: #555; text-decoration: none; margin-right: 5px; }
        .work-links a:hover { background: #f8f8f8; }
      </style>

      <!-- 1. V-LGP -->
      <div class="work-item">
        <div class="work-img">
          <img src="{{ 'assets/img/vlgp.gif' | relative_url }}" alt="V-LGP">
        </div>
        <div class="work-content">
          <div class="work-title">V-LGP: Vision-Language Geometric Programming for Long-Horizon Assembly</div>
          <div class="work-venue">Under Review at IEEE Robotics and Automation Letters (RA-L)</div>
          <div class="work-desc">
            A hierarchical framework bridging VLM reasoning with low-level LGP solvers. Enhanced the C++ KOMO solver with virtual anchors for multi-support consistency.
          </div>
          <div class="work-links">
            <a href="https://github.com/LeslieLinXinxiang/VLM-LGP">Code</a>
            <a style="color: #999; border-color: #eee;">PDF (Coming Soon)</a>
          </div>
        </div>
      </div>

      <!-- 2. VLM Agent -->
      <div class="work-item">
        <div class="work-img">
          <img src="{{ 'assets/img/vlm_agent.gif' | relative_url }}" alt="VLM Agent">
        </div>
        <div class="work-content">
          <div class="work-title">Neuro-Symbolic Agent for Dexterous Manipulation</div>
          <div class="work-venue">Project | Lingxin Dexterous Hand Integration</div>
          <div class="work-desc">
            End-to-end deployment of VLM agents on a 7-DOF arm. Solved contact-stability issues in real-world logic tasks through motor torque profile optimization.
          </div>
          <div class="work-links">
            <a href="https://github.com/LeslieLinXinxiang/VLM-Game-Agent">Code</a>
          </div>
        </div>
      </div>

      <!-- 3. Humanoid -->
      <div class="work-item">
        <div class="work-img">
          <img src="{{ 'assets/img/collaboration_project.jpg' | relative_url }}" alt="Humanoid">
        </div>
        <div class="work-content">
          <div class="work-title">Mechatronic Design for Bipedal Humanoid Joints</div>
          <div class="work-venue">Industry Collaboration with Greenland Harmonic Drive</div>
          <div class="work-desc">
            Developed high-torque density joint modules. Performed HIL testing and vibration analysis to mitigate mechanical resonance for locomotion stability.
          </div>
        </div>
      </div>
      <!-- 修正：删除了多余的 <div> 开启标签，补充了闭合标签 -->
    </div>
  </article>
</div>
