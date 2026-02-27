---
layout: page
permalink: /projects/
title: projects
nav: true
nav_order: 3
---

<!-- 1. Top Gallery (Visual Impact) -->
<div class="row mb-5">
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/IMG_8133.JPG" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/Abstract.png" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/constant_force.jpg" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

<div class="projects">
  <div class="alert alert-light text-center" role="alert" style="font-size: 0.9rem; color: #666; letter-spacing: 1px;">
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
          <img src="{{ item.img | relative_url }}" class="img-fluid rounded border">
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
  <!-- At Dreame (Mova)        -->
  <!-- ======================= -->
  <h3 class="mt-4 mb-3">At Dreame Technology</h3>
  <div class="row">
    <div class="col-sm-6">
      <!-- Mova Carousel -->
      <div id="dreameCarousel" class="carousel slide" data-ride="carousel" data-interval="3000">
        <div class="carousel-inner rounded z-depth-1">
          <div class="carousel-item active">
            <img class="d-block w-100" src="{{ 'assets/img/MOVA_Mower-1000Thumb_1.jpg' | relative_url }}" alt="Mova Mower">
          </div>
          <div class="carousel-item">
            <img class="d-block w-100" src="{{ 'assets/img/mova_blade.png' | relative_url }}" alt="Blade Module">
          </div>
        </div>
        <a class="carousel-control-prev" href="#dreameCarousel" role="button" data-slide="prev">
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="sr-only">Previous</span>
        </a>
        <a class="carousel-control-next" href="#dreameCarousel" role="button" data-slide="next">
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="sr-only">Next</span>
        </a>
      </div>
    </div>
    <div class="col-sm-6">
      <h5 style="font-weight: 600;">MOVA M1 Outdoor Mowing Robot</h5>
      <p style="text-align: justify;">
        <b>Mobile Robotics Platform.</b> Led the precision design and dynamic balancing of the blade actuation module. Resolved IPX-rated waterproofing and vibration compensation for harsh outdoor environments. 
        <br>
        <i>Key Achievement:</i> Supported a global shipment target of 200,000+ units.
      </p>
    </div>
  </div>

  <hr>

  <!-- ======================= -->
  <!-- At Laifen               -->
  <!-- ======================= -->
  <h3 class="mt-4 mb-3">At Laifen Technology</h3>
  <div class="row">
    <div class="col-sm-5">
      {% include figure.liquid path="assets/img/constant_force.jpg" class="img-fluid rounded border" %}
    </div>
    <div class="col-sm-7">
      <h5 style="font-weight: 600;">Constant Force Lifting Mechanism</h5>
      <p style="text-align: justify;">
        Engineered a gravity-compensation mechanism using scotch yoke and cam profiles to linearize spring output. This innovation allows users to adjust heavy device height with zero effort (hovering effect).
      </p>
      <a href="{{ 'assets/pdf/CN202420998035_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-outline-primary btn-sm">
        <i class="fas fa-file-pdf"></i> CN 202420998035 U
      </a>
    </div>
  </div>

  <hr>

  <!-- ======================= -->
  <!-- At EcoFlow              -->
  <!-- ======================= -->
  <h3 class="mt-4 mb-3">At EcoFlow</h3>
  
  <!-- Project 1: Blade Mower -->
  <div class="row mb-4">
    <div class="col-sm-6">
      <!-- Ecoflow Carousel -->
      <div id="ecoflowCarousel" class="carousel slide" data-ride="carousel" data-interval="3000">
        <div class="carousel-inner rounded z-depth-1">
          <div class="carousel-item active">
            <img class="d-block w-100" src="{{ 'assets/img/blade_3d_model.PNG' | relative_url }}" alt="3D Model">
          </div>
          <div class="carousel-item">
            <img class="d-block w-100" src="{{ 'assets/img/blade with puppy.JPG' | relative_url }}" alt="Real Product">
          </div>
          <div class="carousel-item">
            <img class="d-block w-100" src="{{ 'assets/img/IMG_8133.JPG' | relative_url }}" alt="Testing">
          </div>
        </div>
        <a class="carousel-control-prev" href="#ecoflowCarousel" role="button" data-slide="prev">
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="sr-only">Previous</span>
        </a>
        <a class="carousel-control-next" href="#ecoflowCarousel" role="button" data-slide="next">
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="sr-only">Next</span>
        </a>
      </div>
    </div>
    <div class="col-sm-6">
      <h5 style="font-weight: 600;">Blade Robotic Lawn Mower</h5>
      <p style="text-align: justify;">
        <b>CES Innovation Award Winner.</b> Led the structural development of the mowing deck and leaf collection module. Optimized the gear transmission system, extending service life by 40%.
      </p>
    </div>
  </div>

  <!-- Project 2: Smart Wagon & Patent Wall -->
  <div class="row">
    <div class="col-sm-12">
      <h5 style="font-weight: 600;">Smart Electric Camping Wagon & Patent Portfolio</h5>
      <p>Implemented current-loop control for gravity compensation (anti-slip on slopes). Authored 5 utility patents for novel actuation structures.</p>
      
      <!-- Patent Wall (Grid) -->
      <div class="row">
        <div class="col-md-4 col-6 mb-2">
          <a href="{{ 'assets/pdf/CN202320491229_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-light btn-sm btn-block border text-left" style="font-size: 0.75rem;">
            <i class="fas fa-certificate text-danger"></i> CN 202320491229 U
          </a>
        </div>
        <div class="col-md-4 col-6 mb-2">
          <a href="{{ 'assets/pdf/CN202320498391_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-light btn-sm btn-block border text-left" style="font-size: 0.75rem;">
            <i class="fas fa-certificate text-danger"></i> CN 202320498391 U
          </a>
        </div>
        <div class="col-md-4 col-6 mb-2">
          <a href="{{ 'assets/pdf/CN202320571565_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-light btn-sm btn-block border text-left" style="font-size: 0.75rem;">
            <i class="fas fa-certificate text-danger"></i> CN 202320571565 U
          </a>
        </div>
        <div class="col-md-4 col-6 mb-2">
          <a href="{{ 'assets/pdf/CN202320574400_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-light btn-sm btn-block border text-left" style="font-size: 0.75rem;">
            <i class="fas fa-certificate text-danger"></i> CN 202320574400 U
          </a>
        </div>
        <div class="col-md-4 col-6 mb-2">
          <a href="{{ 'assets/pdf/CN202320589748_FullTextImage.pdf' | relative_url }}" target="_blank" class="btn btn-light btn-sm btn-block border text-left" style="font-size: 0.75rem;">
            <i class="fas fa-certificate text-danger"></i> CN 202320589748 U
          </a>
        </div>
      </div>
    </div>
  </div>

</div>
