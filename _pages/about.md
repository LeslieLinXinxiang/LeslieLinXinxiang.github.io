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
<style>
  /* 强制锁定学术列表样式，防止主题干扰 */
  .pub-list { margin-top: 30px; }
  .pub-item { display: flex; align-items: flex-start; margin-bottom: 35px; gap: 20px; }
  .pub-img { flex: 0 0 220px; max-width: 220px; } /* 锁定图片宽度 */
  .pub-img img { width: 100%; height: 130px; object-fit: cover; border-radius: 4px; border: 1px solid #f0f0f0; }
  .pub-content { flex: 1; }
  .pub-title { font-size: 1.05rem; font-weight: 600; margin: 0 0 5px 0; color: #333; }
  .pub-authors { font-size: 0.9rem; margin-bottom: 5px; color: #555; }
  .pub-venue { font-size: 0.9rem; font-style: italic; color: #777; margin-bottom: 8px; }
  .pub-desc { font-size: 0.88rem; line-height: 1.4; color: #444; text-align: justify; margin-bottom: 10px; }
  .pub-links a { 
    font-size: 0.75rem; padding: 1px 8px; margin-right: 5px; border-radius: 3px; 
    border: 1px solid #ccc; color: #555; text-decoration: none; 
  }
  .pub-links a:hover { background: #f5f5f5; border-color: #999; }
</style>

<div class="pub-list">
  <h2 style="font-size: 1.5rem; border-bottom: 1.5px solid #333; padding-bottom: 8px; margin-bottom: 25px;">Selected Research</h2>

  <!-- 1. V-LGP -->
  <div class="pub-item">
    <div class="pub-img">
      <img src="{{ 'assets/img/vlgp.gif' | relative_url }}" alt="V-LGP">
    </div>
    <div class="pub-content">
      <div class="pub-title">V-LGP: Vision-Language Geometric Programming for Long-Horizon Assembly</div>
      <div class="pub-authors"><b>Xinxiang Lin</b>, et al.</div>
      <div class="pub-venue">Under Review at IEEE Robotics and Automation Letters (RA-L)</div>
      <div class="pub-desc">
        A hierarchical planning framework that bridges VLM-based semantic reasoning with low-level KOMO geometric solvers. Enhanced the solver with virtual anchors to resolve multi-support stability.
      </div>
      <div class="pub-links">
        <a href="https://github.com/LeslieLinXinxiang/VLM-LGP">Code</a>
        <a style="color: #999; border-color: #eee;">PDF (Coming Soon)</a>
      </div>
    </div>
  </div>

  <!-- 2. VLM Agent -->
  <div class="pub-item">
    <div class="pub-img">
      <img src="{{ 'assets/img/vlm_agent.gif' | relative_url }}" alt="VLM Agent">
    </div>
    <div class="pub-content">
      <div class="pub-title">Neuro-Symbolic Tabletop Agent with Dexterous Manipulation</div>
      <div class="pub-authors"><b>Xinxiang Lin</b>, et al.</div>
      <div class="pub-venue">Technical Report / University Project</div>
      <div class="pub-desc">
        End-to-end deployment of a VLM reasoning agent on a 7-DOF arm with Lingxin Dexterous Hands. Solved Sim-to-Real gaps in high-precision contact-rich tasks like Tic-Tac-Toe.
      </div>
      <div class="pub-links">
        <a href="https://github.com/LeslieLinXinxiang/VLM-Game-Agent">Code</a>
      </div>
    </div>
  </div>

  <!-- 3. Humanoid -->
  <div class="pub-item">
    <div class="pub-img">
      <img src="{{ 'assets/img/collaboration_project.jpg' | relative_url }}" alt="Humanoid">
    </div>
    <div class="pub-content">
      <div class="pub-title">System Integration and Mechatronic Design for Bipedal Humanoid Joints</div>
      <div class="pub-authors"><b>Xinxiang Lin</b>, et al.</div>
      <div class="pub-venue">Industry Collaboration with Greenland Harmonic Drive</div>
      <div class="pub-desc">
        Developed high-torque joint modules and performed HIL testing. Mitigated mechanical resonance through vibration analysis to ensure locomotion stability on real hardware.
      </div>
    </div>
  </div>
</div>
