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
  /* 1. Gallery & Box Styles */
  .gallery-box {
    height: 180px; width: 100%; display: flex; align-items: center; justify-content: center;
    background-color: #fcfcfc; border: 1px solid #f0f0f0; border-radius: 5px; margin-bottom: 10px;
  }
  .gallery-box img { max-height: 100%; max-width: 100%; object-fit: contain; }

  /* Carousel Box: 320px height locked */
  .carousel-contain-box {
    height: 320px; width: 100%; display: flex; align-items: center; justify-content: center;
    background-color: #f8f9fa; border: 1px solid #eee; border-radius: 5px;
  }
  .carousel-contain-box img { max-height: 100%; max-width: 100%; object-fit: contain; }
  
  /* Static Box: 250px height locked */
  .static-contain-box {
    height: 250px; width: 100%; display: flex; align-items: center; justify-content: center;
    background-color: #fff; border: 1px solid #eee; border-radius: 5px;
  }
  .static-contain-box img { max-height: 100%; max-width: 100%; object-fit: contain; }

  /* 2. Patent Button Style (Matches Smart Wagon) */
  .btn-patent {
    font-size: 0.7rem !important; 
    padding: 4px 8px !important; 
    margin-bottom: 5px;
    white-space: nowrap; 
    overflow: hidden; 
    text-overflow: ellipsis; 
    text-align: left;
    border: 1px solid #007bff !important; 
    color: #007bff !important;
    background-color: white;
    border-radius: 0.2rem;
    display: inline-block;
  }
  .btn-patent:hover { 
    background-color: #007bff !important; 
    color: white !important; 
    text-decoration: none;
  }
  /* Grid version specifically for Smart Wagon list */
  .btn-patent-block {
    width: 100%;
  }

  /* 3. Typography */
  h5 { font-weight: 700; font-size: 1.1rem; color: #333; margin-bottom: 8px; margin-top: 0; }
  p.desc-text { font-size: 0.9rem; line-height: 1.5; color: #444; text-align: justify; margin-bottom: 10px; }
  
  /* Description Header Style */
  header.post-header { margin-bottom: 40px !important; }
  p.post-description { font-size: 1.1rem; color: #828282; margin-top: -10px; margin-bottom: 30px; font-weight: 300; }
</style>

<!-- 1. Top Gallery -->
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
          <h5>{{ item.title }}</h5>
          <p class="desc-text">{{ item.desc }}</p>
          {% if item.code %}
          <a href="{{ item.code }}" class="btn btn-outline-dark btn-sm">Code</a>
          {% endif %}
        </div>
      </div>
    {% endif %}
  {% endfor %}

  <hr>

  <!-- At Dreame (Layout Fixed to 5:7) -->
  <h3 class="mt-4 mb-4">At Dreame Technology</h3>
  <div class="row mb-5">
    <div class="col-sm-5">
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
    <div class="col-sm-7">
      <h5>MOVA Robotic Lawn Mower</h5>
      <p class="desc-text">
        <b>Mobile Robotics Platform.</b> Led the precision design and dynamic balancing of the blade actuation module. Resolved IPX-rated waterproofing and vibration compensation for harsh outdoor environments. 
        <br><i>Key Achievement:</i> Supported global shipment of 200,000+ units.
      </p>
    </div>
  </div>

  <hr>

  <!-- At Laifen (Button Style Fixed) -->
  <h3 class="mt-4 mb-4">At Laifen Technology</h3>
  <div class="row mb-5">
    <div class="col-sm-5">
      <div class="static-contain-box">
        <img src="{{ 'assets/img/constant_force.jpg' | relative_url }}" alt="Gravity Compensation">
      </div>
    </div>
    <div class="col-sm-7">
      <h5>Constant Force Lifting Mechanism</h5>
      <p class="desc-text">
        Engineered a gravity-compensation mechanism using scotch yoke and cam profiles to linearize spring output. This innovation allows users to adjust heavy device height with zero effort (hovering effect).
      </p>
      <!-- Short Button, Blue Style -->
      <div style="margin-top: 10px;">
        <a href="{{ 'assets/pdf/CN202420998035_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn-patent">
          <i class="fas fa-file-pdf"></i> CN 202420998035 U
        </a>
      </div>
    </div>
  </div>

  <hr>

  <!-- At EcoFlow (Layout Fixed to 5:7) -->
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
          <div class="carousel-item active"><div class="carousel-contain-box"><img src="{{ 'assets/img/blade_3d_model.PNG' | relative_url }}"></div></div>
          <div class="carousel-item"><div class="carousel-contain-box"><img src="{{ 'assets/img/blade with puppy.JPG' | relative_url }}"></div></div>
          <div class="carousel-item"><div class="carousel-contain-box"><img src="{{ 'assets/img/IMG_8133.JPG' | relative_url }}"></div></div>
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
      <div class="static-contain-box">
        <img src="{{ 'assets/img/Abstract.png' | relative_url }}" alt="Wagon Structure">
      </div>
    </div>
    <div class="col-sm-7">
      <h5>Smart Electric Camping Wagon</h5>
      <p class="desc-text">
        Spearheaded the development of a smart electric-assist camping wagon aimed at redefining outdoor heavy-payload transport. Engineered a compact folding kinematic architecture and implemented dynamic current-loop control for gravity compensation. This system provides users with seamless, effortless propulsion and critical anti-slip safety on slopes, significantly enhancing the overall user experience.
      </p>
      
      <!-- Patent Grid -->
      <div class="row mt-2">
        <div class="col-md-6 col-12"><a href="{{ 'assets/pdf/CN202320491229_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn-patent btn-patent-block"><i class="fas fa-file-pdf"></i> CN 202320491229 U</a></div>
        <div class="col-md-6 col-12"><a href="{{ 'assets/pdf/CN202320498391_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn-patent btn-patent-block"><i class="fas fa-file-pdf"></i> CN 202320498391 U</a></div>
        <div class="col-md-6 col-12"><a href="{{ 'assets/pdf/CN202320571565_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn-patent btn-patent-block"><i class="fas fa-file-pdf"></i> CN 202320571565 U</a></div>
        <div class="col-md-6 col-12"><a href="{{ 'assets/pdf/CN202320574400_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn-patent btn-patent-block"><i class="fas fa-file-pdf"></i> CN 202320574400 U</a></div>
        <div class="col-md-6 col-12"><a href="{{ 'assets/pdf/CN202320589748_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn-patent btn-patent-block"><i class="fas fa-file-pdf"></i> CN 202320589748 U</a></div>
      </div>
    </div>
  </div>

</div>
