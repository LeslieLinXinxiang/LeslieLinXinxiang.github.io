---
layout: page
title: Projects
permalink: /projects/
description: A selection of research and engineering projects.
nav: true
display_categories: [Research, Industry]
horizontal: false
---

<!-- V-LGP Project -->
<div class="projects">
  <h2 class="category">Research</h2>
<!--  {% include repository/repo.html repository="LeslieLinXinxiang/VLM-LGP" %} -->
</div>

<div class="container">
  <div class="row">
    <div class="card-item col-sm-12">
      <div class="card sticky-teaser mb-3">
        <div class="row no-gutters">
          <div class="col-md-6">
            {% include figure.html path="assets/img/vlgp.gif" title="V-LGP Demo" class="img-fluid rounded-left" %}
          </div>
          <div class="col-md-6">
            <div class="card-body">
              <h3 class="card-title">V-LGP: Vision-Language Geometric Programming</h3>
              <p class="card-text"><b>Status:</b> In Preparation for IEEE RAL.</p>
              <p class="card-text">A hierarchical framework bridging VLM reasoning with low-level LGP solvers for long-horizon robotic assembly. Developed a custom C++ KOMO solver enhancement to handle multi-support physics constraints.</p>
              <div class="row ml-1">
                <a href="https://github.com/LeslieLinXinxiang/VLM-LGP" class="btn btn-outline-dark btn-sm">Code</a>
                <span class="btn btn-outline-secondary btn-sm disabled">PDF (Coming Soon)</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

<!-- VLM Agent Project -->
  <div class="row">
    <div class="card-item col-sm-12">
      <div class="card sticky-teaser mb-3">
        <div class="row no-gutters">
          <div class="col-md-6">
            {% include figure.html path="assets/img/vlm_agent.gif" title="VLM Agent" class="img-fluid rounded-left" %}
          </div>
          <div class="col-md-6">
            <div class="card-body">
              <h3 class="card-title">Multimodal Game Agent with Dexterous Hand</h3>
              <p class="card-text">Integrated an end-to-end VLM agent with a <b>Lingxin Dexterous Hand</b>. Solved Sim-to-Real stability issues in precision grasping and tabletop game logic execution.</p>
              <div class="row ml-1">
                <a href="https://github.com/LeslieLinXinxiang/VLM-Game-Agent" class="btn btn-outline-dark btn-sm">Code</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

<!-- Humanoid Project -->
  <h2 class="category">Industry</h2>
  <div class="row">
    <div class="card-item col-sm-12">
      <div class="card sticky-teaser mb-3">
        <div class="row no-gutters">
          <div class="col-md-4">
            {% include figure.html path="assets/img/collaboration_project.jpg" title="Humanoid Project" class="img-fluid rounded-left" %}
          </div>
          <div class="col-md-8">
            <div class="card-body">
              <h3 class="card-title">Humanoid Robot Joint & System Integration</h3>
              <p class="card-text"><b>Collaboration with Greenland Harmonic Drive.</b></p>
              <p class="card-text">Focused on the mechatronic design of high-torque density joints. Assisted in whole-body control deployment and hardware-in-the-loop (HIL) testing for the bipedal platform.</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
