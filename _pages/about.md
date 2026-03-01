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

<!-- 2. Selected Works Section -->
    <div class="selected-works" style="margin-top: 50px;">
      <h2 style="font-size: 1.5rem; border-bottom: 1.5px solid #333; padding-bottom: 8px; margin-bottom: 25px;">Selected Works</h2>
      
      <style>
        /* 这里的 CSS 用于统一样式，布局交给下方的 Bootstrap 类 */
        .work-img-box {
          height: 180px; width: 100%; display: flex; align-items: center; justify-content: center;
          background-color: #fcfcfc; border: 1px solid #f0f0f0; border-radius: 4px; overflow: hidden;
        }
        .work-img-box img { max-height: 100%; max-width: 100%; object-fit: contain; }
        .work-title { font-size: 1.05rem; font-weight: 600; margin: 0 0 5px 0; color: #333; }
        .work-venue { font-size: 0.85rem; color: #777; margin-bottom: 8px; font-style: italic; }
        .work-desc { font-size: 0.88rem; line-height: 1.45; color: #444; text-align: justify; }
        .work-links { margin-top: 8px; }
        .btn-code { font-size: 0.75rem; padding: 2px 8px; border: 1px solid #333; border-radius: 3px; color: #333 !important; background-color: #fff; text-decoration: none; margin-right: 5px; display: inline-block; }
        .btn-pdf-soon { font-size: 0.75rem; padding: 2px 8px; border: 1px solid #d32f2f; border-radius: 3px; color: #d32f2f; background-color: #fff; opacity: 0.8; }
        .btn-patent { font-size: 0.75rem; padding: 2px 8px; border: 1px solid #007bff; border-radius: 3px; color: #007bff !important; text-decoration: none; display: inline-block; }
      </style>

      <!-- 1. V-LGP -->
      <div class="row mb-5">
        <div class="col-sm-5 col-md-4">
          <div class="work-img-box"><img src="{{ 'assets/img/vlgp.gif' | relative_url }}" alt="V-LGP"></div>
        </div>
        <div class="col-sm-7 col-md-8">
          <div class="work-title">V-LGP: Vision-Language Geometric Programming for Long-Horizon Assembly</div>
          <div class="work-venue">Submitted to IEEE Robotics and Automation Letters (RA-L)</div>
          <div class="work-desc">A hierarchical framework bridging VLM reasoning with low-level LGP solvers. Enhanced the C++ KOMO solver with virtual anchors for multi-support consistency.</div>
          <div class="work-links">
            <a href="https://github.com/LeslieLinXinxiang/VLM-LGP" class="btn-code">Code</a>
            <span class="btn-pdf-soon">PDF (Coming Soon)</span>
          </div>
        </div>
      </div>

      <!-- 2. Linkerbot -->
      <div class="row mb-5">
        <div class="col-sm-5 col-md-4">
          <div class="work-img-box"><img src="{{ 'assets/img/vlm_agent.gif' | relative_url }}" alt="VLM Agent"></div>
        </div>
        <div class="col-sm-7 col-md-8">
          <div class="work-title">End-to-End Reasoning for Long-Horizon Autonomous Robotic Manipulation</div>
          <div class="work-venue">Collaboration with Linkerbot | Joint Lab Project</div>
          <div class="work-desc">Developed a vision-centric closed-loop agent for autonomous long-horizon manipulation. Implemented zero-shot multi-modal spatial grounding and adaptive grasping for Linkerhand O6.</div>
          <div class="work-links"><a href="https://github.com/LeslieLinXinxiang/VLM-Game-Agent" class="btn-code">Code</a></div>
        </div>
      </div>

      <!-- 3. Leaderdrive -->
      <div class="row mb-5">
        <div class="col-sm-5 col-md-4">
          <div class="work-img-box"><img src="{{ 'assets/img/collaboration_project.jpg' | relative_url }}" alt="Humanoid"></div>
        </div>
        <div class="col-sm-7 col-md-8">
          <div class="work-title">Mechatronic Design and Locomotion Deployment for Bipedal Humanoid</div>
          <div class="work-venue">Industry Collaboration with Leaderdrive</div>
          <div class="work-desc">Collaborated on mechatronic development of a bipedal platform. Executed joint module design and assisted in real-machine deployment of locomotion algorithms.</div>
        </div>
      </div>

      <!-- 4. MOVA M1 -->
      <div class="row mb-5">
        <div class="col-sm-5 col-md-4">
          <div class="work-img-box"><img src="{{ 'assets/img/MOVA_Mower-1000Thumb_1.jpg' | relative_url }}" alt="MOVA M1"></div>
        </div>
        <div class="col-sm-7 col-md-8">
          <div class="work-title">MOVA Robotic Lawn Mower</div>
          <div class="work-venue">Dreame Technology | Mobile Robotics</div>
          <div class="work-desc">Led precision design and dynamic balancing of the blade module. Resolved IPX waterproofing and vibration compensation for global mass production.</div>
        </div>
      </div>

      <!-- 5. Laifen -->
      <div class="row mb-5">
        <div class="col-sm-5 col-md-4">
          <div class="work-img-box"><img src="{{ 'assets/img/constant_force.jpg' | relative_url }}" alt="Constant Force"></div>
        </div>
        <div class="col-sm-7 col-md-8">
          <div class="work-title">Constant Force Lifting Mechanism</div>
          <div class="work-venue">Laifen Technology | Lead Inventor</div>
          <div class="work-desc">Engineered a gravity-compensation mechanism using scotch yoke and cam profiles to linearize spring output, achieving zero-effort height adjustment.</div>
          <div class="work-links">
            <a href="{{ 'assets/pdf/CN202420998035_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn-patent">CN 202420998035 U</a>
          </div>
        </div>
      </div>



    </div>
  </article>
</div>
