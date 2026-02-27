---
layout: page
permalink: /projects/
title: projects
nav: true
nav_order: 2
description: A collection of projects during my work and study.
---

<!-- =====================================================================
     CUSTOM CSS
     ===================================================================== -->
<style>
  /* 强制隐藏默认生成的 Page Title，我们自己手写以控制样式 */
  /* 注意：al-folio 默认会在 layout 中生成标题，我们这里用 CSS 微调 description 的位置 */
  
  /* 图片容器样式 (保持不变) */
  .gallery-box {
    height: 180px; width: 100%; display: flex; align-items: center; justify-content: center;
    background-color: #fcfcfc; border: 1px solid #f0f0f0; border-radius: 5px; margin-bottom: 10px;
  }
  .gallery-box img { max-height: 100%; max-width: 100%; object-fit: contain; }

  .carousel-contain-box {
    height: 320px; width: 100%; display: flex; align-items: center; justify-content: center;
    background-color: #f8f9fa; border: 1px solid #eee; border-radius: 5px;
  }
  .carousel-contain-box img { max-height: 100%; max-width: 100%; object-fit: contain; }
  
  .static-contain-box {
    height: 250px; width: 100%; display: flex; align-items: center; justify-content: center;
    background-color: #fff; border: 1px solid #eee; border-radius: 5px;
  }
  .static-contain-box img { max-height: 100%; max-width: 100%; object-fit: contain; }

  .btn-patent {
    font-size: 0.7rem !important; padding: 4px 6px !important; margin-bottom: 5px;
    white-space: nowrap; overflow: hidden; text-overflow: ellipsis; width: 100%; text-align: left;
    border-color: #007bff !important; color: #007bff !important;
  }
  .btn-patent:hover { background-color: #007bff !important; color: white !important; }
  
  /* 调整 Description 的样式，使其更像 Mayank 的风格 */
  header.post-header { margin-bottom: 40px !important; }
  p.post-description { 
    font-size: 1.1rem; 
    color: #828282; 
    margin-top: -10px; 
    margin-bottom: 30px; 
    font-weight: 300;
  }
</style>

<!-- 1. Top Gallery (Moved up, right after header) -->
<div class="row mb-5" style="margin-top: 20px;">
  <div class="col-sm-4 mt-3 mt-md-0">
    <div class="gallery-box"><img src="{{ 'assets/img/IMG_8133.JPG' | relative_url }}" alt="Testing"></div>
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    <div class="gallery-box"><img src="{{ 'assets/img/Abstract.png' | relative_url }}" alt="Mechanism"></div>
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    <div class="gallery-box"><img src="{{ 'assets/img/constant_force.jpg' | relative_url }}" alt="Structure"></div>
  </div>
</div>

<div class="projects">
  <hr>

  <!-- At UM -->
  <h3 class="mt-4 mb-4">At UM</h3>
  {% for item in site.data.works %}
    {% if item.id == 'linkerbot' or item.id == 'leaderdrive' %}
      <div class="row mb-5">
        <div class="col-sm-5">
          <div class="static-contain-box" style="height: 180px;">
            <img src="{{ item.img | relative_url }}" alt="{{ item.title }}">
          </div>
        </div>
        <div class="col-sm-7">
          <h5 style="font-weight: 700;">{{ item.title }}</h5>
          <p style="font-size: 0.9rem; text-align: justify;">{{ item.desc }}</p>
          {% if item.code %}
          <a href="{{ item.code }}" class="btn btn-outline-dark btn-sm">Code</a>
          {% endif %}
        </div>
      </div>
    {% endif %}
  {% endfor %}

  <hr>

  <!-- At Dreame -->
  <h3 class="mt-4 mb-4">At Dreame Technology</h3>
  <div class="row mb-5">
    <div class="col-sm-6">
      <div id="dreameCarousel" class="carousel slide" data-ride="carousel" data-interval="4000">
        <ol class="carousel-indicators">
          <li data-target="#dreameCarousel" data-slide-to="0" class="active"></li>
          <li data-target="#dreameCarousel" data-slide-to="1"></li>
        </ol>
        <div class="carousel-inner rounded">
          <div class="carousel-item active">
            <div class="carousel-contain-box"><img src="{{ 'assets/img/MOVA_Mower-1000Thumb_1.jpg' | relative_url }}"></div>
          </div>
          <div class="carousel-item">
            <div class="carousel-contain-box"><img src="{{ 'assets/img/mova_blade.png' | relative_url }}"></div>
          </div>
        </div>
        <a class="carousel-control-prev" href="#dreameCarousel" role="button" data-slide="prev"><span class="carousel-control-prev-icon" style="filter: invert(1);"></span></a>
        <a class="carousel-control-next" href="#dreameCarousel" role="button" data-slide="next"><span class="carousel-control-next-icon" style="filter: invert(1);"></span></a>
      </div>
    </div>
    <div class="col-sm-6">
      <h5 style="font-weight: 700;">MOVA M1 Outdoor Mowing Robot</h5>
      <p style="font-size: 0.9rem; text-align: justify;">
        <b>Mobile Robotics Platform.</b> Led the precision design and dynamic balancing of the blade actuation module. Resolved IPX-rated waterproofing and vibration compensation.
        <br><i>Key Achievement:</i> Supported global shipment of 200,000+ units.
      </p>
    </div>
  </div>

  <hr>

  <!-- At Laifen -->
  <h3 class="mt-4 mb-4">At Laifen Technology</h3>
  <div class="row mb-5">
    <div class="col-sm-5">
      <div class="static-contain-box">
        <img src="{{ 'assets/img/constant_force.jpg' | relative_url }}" alt="Gravity Compensation">
      </div>
    </div>
    <div class="col-sm-7">
      <h5 style="font-weight: 700;">Constant Force Lifting Mechanism</h5>
      <p style="font-size: 0.9rem; text-align: justify;">
        Engineered a gravity-compensation mechanism using scotch yoke and cam profiles to linearize spring output. This innovation allows users to adjust heavy device height with zero effort (hovering effect).
      </p>
      <div style="margin-top: 10px;">
        <a href="{{ 'assets/pdf/CN202420998035_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-outline-primary btn-patent">
          <i class="fas fa-file-pdf"></i> CN 202420998035 U
        </a>
      </div>
    </div>
  </div>

  <hr>

  <!-- At EcoFlow -->
  <h3 class="mt-4 mb-4">At EcoFlow</h3>
  
  <!-- Project 1: Blade Mower -->
  <div class="row mb-5">
    <div class="col-sm-6">
      <div id="ecoflowCarousel" class="carousel slide" data-ride="carousel" data-interval="4000">
        <ol class="carousel-indicators">
          <li data-target="#ecoflowCarousel" data-slide-to="0" class="active"></li>
          <li data-target="#ecoflowCarousel" data-slide-to="1"></li>
          <li data-target="#ecoflowCarousel" data-slide-to="2"></li>
        </ol>
        <div class="carousel-inner rounded">
          <div class="carousel-item active"><div class="carousel-contain-box"><img src="{{ 'assets/img/blade_3d_model.PNG' | relative_url }}"></div></div>
          <div class="carousel-item"><div class="carousel-contain-box"><img src="{{ 'assets/img/blade with puppy.JPG' | relative_url }}"></div></div>
          <div class="carousel-item"><div class="carousel-contain-box"><img src="{{ 'assets/img/IMG_8133.JPG' | relative_url }}"></div></div>
        </div>
        <a class="carousel-control-prev" href="#ecoflowCarousel" role="button" data-slide="prev"><span class="carousel-control-prev-icon" style="filter: invert(1);"></span></a>
        <a class="carousel-control-next" href="#ecoflowCarousel" role="button" data-slide="next"><span class="carousel-control-next-icon" style="filter: invert(1);"></span></a>
      </div>
    </div>
    <div class="col-sm-6">
      <h5 style="font-weight: 700;">Blade Robotic Lawn Mower</h5>
      <p style="font-size: 0.9rem; text-align: justify;">
        <b>CES Innovation Award Winner.</b> Led the structural development of the mowing deck and leaf collection module. Optimized the gear transmission system, extending service life by 40%.
      </p>
    </div>
  </div>

  <!-- Project 2: Smart Wagon -->
  <div class="row">
    <div class="col-sm-5">
      <div class="static-contain-box">
        <img src="{{ 'assets/img/Abstract.png' | relative_url }}" alt="Wagon Structure">
      </div>
    </div>
    <div class="col-sm-7">
      <h5 style="font-weight: 700;">Smart Electric Camping Wagon</h5>
      <p style="font-size: 0.9rem; text-align: justify;">
        Implemented current-loop control for gravity compensation (anti-slip on slopes) and designed the folding kinematic structure. Authored 5 utility patents for novel actuation structures.
      </p>
      
      <div class="row mt-3">
        <div class="col-md-6 col-12"><a href="{{ 'assets/pdf/CN202320491229_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-outline-primary btn-patent"><i class="fas fa-file-pdf"></i> CN 202320491229 U</a></div>
        <div class="col-md-6 col-12"><a href="{{ 'assets/pdf/CN202320498391_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-outline-primary btn-patent"><i class="fas fa-file-pdf"></i> CN 202320498391 U</a></div>
        <div class="col-md-6 col-12"><a href="{{ 'assets/pdf/CN202320571565_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-outline-primary btn-patent"><i class="fas fa-file-pdf"></i> CN 202320571565 U</a></div>
        <div class="col-md-6 col-12"><a href="{{ 'assets/pdf/CN202320574400_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-outline-primary btn-patent"><i class="fas fa-file-pdf"></i> CN 202320574400 U</a></div>
        <div class="col-md-6 col-12"><a href="{{ 'assets/pdf/CN202320589748_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-outline-primary btn-patent"><i class="fas fa-file-pdf"></i> CN 202320589748 U</a></div>
      </div>
    </div>
  </div>

</div>
