---
layout: page
permalink: /projects/
title: projects
nav: true
nav_order: 2
---

<!-- =====================================================================
     CUSTOM CSS FOR PIXEL-PERFECT UNIFORMITY
     ===================================================================== -->
<style>
  /* 统一所有图片容器的高度为 180px */
  .unified-box {
    height: 180px;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #fcfcfc;
    border: 1px solid #f0f0f0;
    border-radius: 5px;
    margin-bottom: 0; /* Remove bottom margin to align with text */
  }
  .unified-box img {
    max-height: 100%;
    max-width: 100%;
    object-fit: contain; /* 保证图片完整显示，不裁切 */
  }

  /* 专利按钮样式 */
  .btn-patent {
    font-size: 0.7rem !important;
    padding: 3px 8px !important;
    margin-bottom: 5px;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    width: 100%;
    text-align: left;
    border-color: #007bff !important; /* 强制徕芬蓝 */
    color: #007bff !important;
  }
  .btn-patent:hover {
    background-color: #007bff !important;
    color: white !important;
  }
  
  /* 项目标题微调 */
  h5 { font-weight: 700; font-size: 1.1rem; color: #333; margin-bottom: 8px; }
  /* 描述文本微调 */
  p.desc-text { font-size: 0.9rem; line-height: 1.5; color: #444; text-align: justify; margin-bottom: 10px; }
</style>

<!-- ======================= -->
<!-- 1. Top Gallery          -->
<!-- ======================= -->
<div class="row mb-5">
  <div class="col-sm-4 mt-3 mt-md-0">
    <div class="unified-box">
      <img src="{{ 'assets/img/IMG_8133.JPG' | relative_url }}" alt="Testing">
    </div>
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    <div class="unified-box">
      <img src="{{ 'assets/img/Abstract.png' | relative_url }}" alt="Mechanism">
    </div>
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    <div class="unified-box">
      <img src="{{ 'assets/img/constant_force.jpg' | relative_url }}" alt="Structure">
    </div>
  </div>
</div>

<div class="projects">
  <div class="alert alert-light text-center" role="alert" style="font-size: 0.9rem; color: #666; letter-spacing: 1px; border: 1px solid #eee;">
    A COLLECTION OF PROJECTS DURING MY WORK AND STUDY
  </div>

  <hr>

  <!-- ======================= -->
  <!-- At UM (Academic)        -->
  <!-- ======================= -->
  <h3 class="mt-4 mb-4">At UM</h3>
  
  <!-- 1. Linkerbot -->
  {% for item in site.data.works %}
    {% if item.id == 'linkerbot' %}
      <div class="row mb-5">
        <div class="col-sm-5">
          <div class="unified-box">
            <img src="{{ item.img | relative_url }}" alt="{{ item.title }}">
          </div>
        </div>
        <div class="col-sm-7">
          <h5>{{ item.title }}</h5>
          <p class="desc-text">{{ item.desc }}</p>
          <a href="{{ item.code }}" class="btn btn-outline-dark btn-sm">Code</a>
        </div>
      </div>
    {% endif %}
  {% endfor %}

  <!-- 2. Leaderdrive Humanoid (Added as requested) -->
  {% for item in site.data.works %}
    {% if item.id == 'leaderdrive' %}
      <div class="row mb-5">
        <div class="col-sm-5">
          <div class="unified-box">
            <img src="{{ item.img | relative_url }}" alt="{{ item.title }}">
          </div>
        </div>
        <div class="col-sm-7">
          <h5>{{ item.title }}</h5>
          <p class="desc-text">{{ item.desc }}</p>
        </div>
      </div>
    {% endif %}
  {% endfor %}

  <hr>

  <!-- ======================= -->
  <!-- At Dreame Technology    -->
  <!-- ======================= -->
  <h3 class="mt-4 mb-4">At Dreame Technology</h3>
  <div class="row mb-5">
    <div class="col-sm-5">
      <!-- Mova Carousel (Height Locked to 180px) -->
      <div id="dreameCarousel" class="carousel slide" data-ride="carousel" data-interval="4000">
        <ol class="carousel-indicators">
          <li data-target="#dreameCarousel" data-slide-to="0" class="active"></li>
          <li data-target="#dreameCarousel" data-slide-to="1"></li>
        </ol>
        <div class="carousel-inner rounded">
          <div class="carousel-item active">
            <div class="unified-box">
              <img src="{{ 'assets/img/MOVA_Mower-1000Thumb_1.jpg' | relative_url }}" alt="Mova Mower">
            </div>
          </div>
          <div class="carousel-item">
            <div class="unified-box">
              <img src="{{ 'assets/img/mova_blade.png' | relative_url }}" alt="Blade Module">
            </div>
          </div>
        </div>
        <a class="carousel-control-prev" href="#dreameCarousel" role="button" data-slide="prev">
          <span class="carousel-control-prev-icon" style="filter: invert(1);"></span>
        </a>
        <a class="carousel-control-next" href="#dreameCarousel" role="button" data-slide="next">
          <span class="carousel-control-next-icon" style="filter: invert(1);"></span>
        </a>
      </div>
    </div>
    <div class="col-sm-7">
      <h5>MOVA 600&1000 Robotic Lawn Mower</h5>
      <p class="desc-text">
        <b>Mobile Robotics.</b> Led the precision design and dynamic balancing of the blade actuation module. Resolved IPX-rated waterproofing and vibration compensation for harsh outdoor environments. 
        <br>
        <i>Key Achievement:</i> Supported a global shipment target of 200,000+ units.
      </p>
    </div>
  </div>

  <hr>

  <!-- ======================= -->
  <!-- At Laifen Technology    -->
  <!-- ======================= -->
  <h3 class="mt-4 mb-4">At Laifen Technology</h3>
  <div class="row mb-5">
    <div class="col-sm-5">
      <div class="unified-box">
        <img src="{{ 'assets/img/constant_force.jpg' | relative_url }}" alt="Gravity Compensation">
      </div>
    </div>
    <div class="col-sm-7">
      <h5>Constant Force Lifting Mechanism</h5>
      <p class="desc-text">
        Engineered a gravity-compensation mechanism using scotch yoke and cam profiles to linearize spring output. This innovation allows users to adjust heavy device height with zero effort (hovering effect).
      </p>
      <div style="max-width: 200px;">
        <a href="{{ 'assets/pdf/CN202420998035_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-outline-primary btn-patent">
          <i class="fas fa-file-pdf"></i> CN 202420998035 U
        </a>
      </div>
    </div>
  </div>

  <hr>

  <!-- ======================= -->
  <!-- At EcoFlow              -->
  <!-- ======================= -->
  <h3 class="mt-4 mb-4">At EcoFlow</h3>
  
  <!-- Project 1: Blade Mower -->
  <div class="row mb-5">
    <div class="col-sm-5">
      <div id="ecoflowCarousel" class="carousel slide" data-ride="carousel" data-interval="4000">
        <ol class="carousel-indicators">
          <li data-target="#ecoflowCarousel" data-slide-to="0" class="active"></li>
          <li data-target="#ecoflowCarousel" data-slide-to="1"></li>
          <li data-target="#ecoflowCarousel" data-slide-to="2"></li>
        </ol>
        <div class="carousel-inner rounded">
          <div class="carousel-item active"><div class="unified-box"><img src="{{ 'assets/img/blade_3d_model.PNG' | relative_url }}"></div></div>
          <div class="carousel-item"><div class="unified-box"><img src="{{ 'assets/img/blade with puppy.JPG' | relative_url }}"></div></div>
          <div class="carousel-item"><div class="unified-box"><img src="{{ 'assets/img/IMG_8133.JPG' | relative_url }}"></div></div>
        </div>
        <a class="carousel-control-prev" href="#ecoflowCarousel" role="button" data-slide="prev"><span class="carousel-control-prev-icon" style="filter: invert(1);"></span></a>
        <a class="carousel-control-next" href="#ecoflowCarousel" role="button" data-slide="next"><span class="carousel-control-next-icon" style="filter: invert(1);"></span></a>
      </div>
    </div>
    <div class="col-sm-7">
      <h5>Blade Robotic Lawn Mower</h5>
      <p class="desc-text">
        <b>CES Innovation Award Winner.</b> Led the structural development of the mowing deck and leaf collection module. Optimized the gear transmission system, extending service life by 40% and ensuring IPX5 waterproofing.
      </p>
    </div>
  </div>

  <!-- Project 2: Smart Wagon -->
  <div class="row mb-5">
    <div class="col-sm-5">
      <div class="unified-box">
        <img src="{{ 'assets/img/Abstract.png' | relative_url }}" alt="Wagon Structure">
      </div>
    </div>
    <div class="col-sm-7">
      <h5>Smart Electric Camping Wagon</h5>
      <p class="desc-text">
        Implemented current-loop control for gravity compensation (anti-slip on slopes) and designed the folding kinematic structure.
      </p>
      
      <!-- Patent Grid -->
      <div class="row mt-2">
        <div class="col-md-6 col-12"><a href="{{ 'assets/pdf/CN202320491229_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-outline-primary btn-patent"><i class="fas fa-file-pdf"></i> CN 202320491229 U</a></div>
        <div class="col-md-6 col-12"><a href="{{ 'assets/pdf/CN202320498391_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-outline-primary btn-patent"><i class="fas fa-file-pdf"></i> CN 202320498391 U</a></div>
        <div class="col-md-6 col-12"><a href="{{ 'assets/pdf/CN202320571565_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-outline-primary btn-patent"><i class="fas fa-file-pdf"></i> CN 202320571565 U</a></div>
        <div class="col-md-6 col-12"><a href="{{ 'assets/pdf/CN202320574400_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-outline-primary btn-patent"><i class="fas fa-file-pdf"></i> CN 202320574400 U</a></div>
        <div class="col-md-6 col-12"><a href="{{ 'assets/pdf/CN202320589748_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-outline-primary btn-patent"><i class="fas fa-file-pdf"></i> CN 202320589748 U</a></div>
      </div>
    </div>
  </div>

</div>
