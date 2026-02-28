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
    <!-- 1. Bio Section -->
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
        /* 1. Code 按钮：黑边白底 */
        .work-links .btn-code { font-size: 0.75rem; padding: 2px 8px; border: 1px solid #333; border-radius: 3px; color: #333; background-color: #fff; text-decoration: none; margin-right: 5px; display: inline-block; }
        .work-links .btn-code:hover { background-color: #333; color: #fff; text-decoration: none; }
        
        /* 2. PDF 按钮：红边白底 */
        .work-links .btn-pdf-soon { font-size: 0.75rem; padding: 2px 8px; border: 1px solid #d32f2f; border-radius: 3px; color: #d32f2f; background-color: #fff; text-decoration: none; margin-right: 5px; display: inline-block; cursor: not-allowed; opacity: 0.8; }
        
        /* 3. Patent 按钮：蓝边白底 (与 Projects 页面统一) */
        .work-links .btn-patent { font-size: 0.75rem; padding: 2px 8px; border: 1px solid #007bff; border-radius: 3px; color: #007bff; text-decoration: none; margin-right: 5px; display: inline-block; background-color: #fff;}
        .work-links .btn-patent:hover { background-color: #007bff; color: #fff; text-decoration: none; }
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
            <a href="https://github.com/LeslieLinXinxiang/VLM-LGP" class="btn-code">Code</a>
            <span class="btn-pdf-soon">PDF (Coming Soon)</span>
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
            <a href="https://github.com/LeslieLinXinxiang/VLM-Game-Agent" class="btn-code">Code</a>
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
            Collaborated on the mechatronic development of a bipedal humanoid platform. Executed the mechanical design of joint modules integrated with high-torque harmonic reducers and assisted in the real-machine deployment of locomotion algorithms. Optimized system stability by identifying and mitigating mechanical resonance issues during 1kHz EtherCAT-based Hardware-in-the-Loop (HIL) testing.
          </div>
        </div>
      </div>

      <!-- 4. Dreame MOVA M1 -->
      <div class="work-item">
        <div class="work-img">
          <img src="{{ 'assets/img/MOVA_Mower-1000Thumb_1.jpg' | relative_url }}" alt="MOVA M1">
        </div>
        <div class="work-content">
          <div class="work-title">MOVA Robotic Lawn Mower</div>
          <div class="work-venue">Dreame Technology | Mobile Robotics Platform</div>
          <div class="work-desc">
            Led the precision design and dynamic balancing of the blade actuation module. Resolved IPX-rated waterproofing and vibration compensation for harsh outdoor environments, supporting a global shipment target of 200,000+ units.
          </div>
        </div>
      </div>

      <!-- 5. Laifen Constant Force -->
      <div class="work-item">
        <div class="work-img">
          <img src="{{ 'assets/img/constant_force.jpg' | relative_url }}" alt="Constant Force">
        </div>
        <div class="work-content">
          <div class="work-title">Constant Force Lifting Mechanism</div>
          <div class="work-venue">Laifen Technology | Lead Inventor</div>
          <div class="work-desc">
            Engineered a gravity-compensation mechanism using scotch yoke and cam profiles to linearize spring output. This innovation allows users to adjust heavy device height with zero effort (hovering effect).
          </div>
          <div class="work-links">
            <a href="{{ 'assets/pdf/CN202420998035_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn-patent">
              <i class="fas fa-file-pdf"></i> CN 202420998035 U
            </a>
          </div>
        </div>
      </div>

      <!-- 6. EcoFlow Blade Mower -->
      <div class="work-item">
        <div class="work-img">
          <img src="{{ 'assets/img/blade with puppy.JPG' | relative_url }}" alt="Blade Mower">
        </div>
        <div class="work-content">
          <div class="work-title">Blade Robotic Lawn Mower System</div>
          <div class="work-venue">EcoFlow | CES Innovation Award Winner</div>
          <div class="work-desc">
            Led the structural development of the mowing deck and leaf collection module. Optimized the gear transmission system, extending service life by 40% and ensuring IPX5 waterproofing.
          </div>
        </div>
      </div>

    </div>
  </article>
</div>
