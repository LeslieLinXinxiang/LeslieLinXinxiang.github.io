---
layout: page
permalink: /projects/
title: projects
nav: true
nav_order: 3
---

<!-- =====================================================================
     CUSTOM CSS FOR UNIFORM LAYOUT (High Signal-to-Noise Ratio)
     ===================================================================== -->
<style>
  /* 1. Top Gallery: Fixed height, NO cropping (Contain) */
  .gallery-box {
    height: 180px;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #fcfcfc; /* Subtle background for non-square images */
    border: 1px solid #f0f0f0;
    border-radius: 5px;
    margin-bottom: 10px;
  }
  .gallery-box img {
    max-height: 100%;
    max-width: 100%;
    object-fit: contain; /* KEY: Ensures full image is visible */
  }

  /* 2. Carousel/Project Images: Fixed height container, NO cropping */
  .carousel-contain-box {
    height: 320px; /* Fixed height for consistency */
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #f8f9fa;
    border: 1px solid #eee;
    border-radius: 5px;
  }
  .carousel-contain-box img {
    max-height: 100%;
    max-width: 100%;
    object-fit: contain;
  }
  
  /* 3. Static Project Images */
  .static-contain-box {
    height: 250px;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #fff;
    border: 1px solid #eee;
    border-radius: 5px;
  }
  .static-contain-box img {
    max-height: 100%;
    max-width: 100%;
    object-fit: contain;
  }

  /* 4. Unified Patent Button Style */
  .btn-patent {
    font-size: 0.75rem !important;
    padding: 4px 8px !important;
    margin-bottom: 5px;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    width: 100%;
    text-align: left;
  }
</style>

<!-- ======================= -->
<!-- 1. Top Gallery          -->
<!-- ======================= -->
<div class="row mb-5">
  <div class="col-sm-4 mt-3 mt-md-0">
    <div class="gallery-box">
      <img src="{{ 'assets/img/IMG_8133.JPG' | relative_url }}" alt="Testing">
    </div>
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    <div class="gallery-box">
      <img src="{{ 'assets/img/Abstract.png' | relative_url }}" alt="Mechanism">
    </div>
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    <div class="gallery-box">
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
  <h3 class="mt-4 mb-3">At UM</h3>
  {% for item in site.data.works %}
    {% if item.id == 'linkerbot' %}
      <div class="row mb-4">
        <div class="col-sm-4">
          <div class="static-contain-box" style="height: 180px;">
            <img src="{{ item.img | relative_url }}" alt="{{ item.title }}">
          </div>
        </div>
        <div class="col-sm-8">
          <h5 style="font-weight: 600;">{{ item.title }}</h5>
          <p>{{ item.desc }}</p>
          <a href="{{ item.code }}" class="btn btn-outline-dark btn-sm">Code</a>
        </div>
      </div>
    {% endif %}
  {% endfor %}

  <hr>

  <!-- ======================= -->
  <!-- At Dreame Technology    -->
  <!-- ======================= -->
  <h3 class="mt-4 mb-3">At Dreame Technology</h3>
  <div class="row">
    <div class="col-sm-6">
      <!-- Mova Carousel -->
      <div id="dreameCarousel" class="carousel slide" data-ride="carousel" data-interval="4000">
        <ol class="carousel-indicators">
          <li data-target="#dreameCarousel" data-slide-to="0" class="active"></li>
          <li data-target="#dreameCarousel" data-slide-to="1"></li>
        </ol>
        <div class="carousel-inner rounded">
          <div class="carousel-item active">
            <div class="carousel-contain-box">
              <img src="{{ 'assets/img/MOVA_Mower-1000Thumb_1.jpg' | relative_url }}" alt="Mova Mower">
            </div>
