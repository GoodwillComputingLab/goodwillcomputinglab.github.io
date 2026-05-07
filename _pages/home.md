---
title: "Goodwill Labs"
layout: homelay
excerpt: "Goodwill Lab at Northeastern University."
sitemap: false
permalink: /
---

<!-- <div class="homepage-intro" markdown="1">

**Goodwill Lab** develops high-performance computing (HPC) and quantum computing systems that are better, more accessible, and useful for solving problems of societal importance.

We also prepare the next generation of students and educators to take advantage of parallel computing systems through research, open-source artifacts, and outreach.

</div> -->

<div class="homepage-hero" markdown="0">
  <h1>Goodwill Lab</h1>

  <p class="hero-subtitle">
    Building better high-performance and quantum computing systems for science and society.
  </p>

  <p class="hero-text">
    The Goodwill Lab develops high-performance computing (HPC) and quantum computing systems
    that are more efficient, accessible, and useful for solving problems of societal importance.
    We also prepare the next generation of students and educators through research,
    open-source artifacts, and outreach.
  </p>

  <div class="hero-cards">
    <div class="hero-card">
      <h3>High-Performance Computing</h3>
      <p>Designing scalable systems, tools, and methods for modern scientific workloads.</p>
    </div>

    <div class="hero-card">
      <h3>Quantum Computing</h3>
      <p>Exploring emerging quantum systems and their role in future computing workflows.</p>
    </div>

    <div class="hero-card">
      <h3>Education & Outreach</h3>
      <p>Creating open-source artifacts and training opportunities for students and educators.</p>
    </div>
  </div>
</div>

<div id="homepageCarousel" class="carousel slide homepage-carousel" data-ride="carousel" data-interval="3000" markdown="0">

  <ol class="carousel-indicators">
    <li data-target="#homepageCarousel" data-slide-to="0" class="active"></li>
    <li data-target="#homepageCarousel" data-slide-to="1"></li>
    <li data-target="#homepageCarousel" data-slide-to="2"></li>
    <li data-target="#homepageCarousel" data-slide-to="3"></li>
    <li data-target="#homepageCarousel" data-slide-to="4"></li>
  </ol>

  <div class="carousel-inner">
    <div class="item active">
      <img src="{{ site.url }}{{ site.baseurl }}/images/datacenter.jpg" alt="Data center">
    </div>
    <div class="item">
      <img src="{{ site.url }}{{ site.baseurl }}/images/alumni.jpg" alt="alumni">
    </div>
    <div class="item">
      <img src="{{ site.url }}{{ site.baseurl }}/images/quantum_computer.jpg" alt="Quantum computer">
    </div>

    <div class="item">
      <img src="{{ site.url }}{{ site.baseurl }}/images/cooling_tower.jpg" alt="cooling">
    </div>

    <div class="item">
      <img src="{{ site.url }}{{ site.baseurl }}/images/neu_campus_cropped.jpg" alt="Northeastern University campus">
    </div>
  </div>


<a class="left carousel-control" href="#homepageCarousel" role="button" data-slide="prev">
  <span style="font-size:42px; color:white;">‹</span>
  <span class="sr-only">Previous</span>
</a>

<a class="right carousel-control" href="#homepageCarousel" role="button" data-slide="next">
  <span style="font-size:42px; color:white;">›</span>
  <span class="sr-only">Next</span>
</a>

</div>

<div class="homepage-lab-footer" markdown="0">
  <a href="http://www.clustrmaps.com/map/Goodwillcomputinglab.github.io" 
     title="Visit tracker for Goodwillcomputinglab.github.io"
     class="visitor-map">
    <img src="//www.clustrmaps.com/map_v2.png?d=3jjPhwShn5KTvAirDB2uR87q9F0ddIlzKPd3HJ1Sq8o" 
         alt="Visitor map">
  </a>

  <div class="neu-logo-block" markdown="0">
    <img src="{{ site.url }}{{ site.baseurl }}/images/sponsorpic/Logo_NEU.jpg" 
         alt="Northeastern University Logo">
  </div>
</div>


<style>
html, body {
  overflow-x: hidden;
}

.homepage-hero {
  width: 100%;
  max-width: 100%;
  box-sizing: border-box;
  padding: 0 0 25px 0;
  margin-bottom: 25px;
}

.homepage-hero h1 {
  margin-top: 0;
}

.hero-subtitle {
  color: #555;
  margin-bottom: 14px;
}

.hero-text {
  line-height: 1.7;
  color: #444;
  max-width: 980px;
  margin-bottom: 26px;
}

.hero-cards {
  display: flex;
  gap: 18px;
  flex-wrap: nowrap;
  box-sizing: border-box;
}

.hero-card {
  flex: 1;
  min-width: 0;
  box-sizing: border-box;
  padding: 18px 20px;
  border-radius: 10px;
  border: 1px solid #e5e7eb;
  border-left: 4px solid #cc0000;
  background: #fcfcfc;
  transition: all 0.2s ease;
}

.hero-card:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 16px rgba(0,0,0,0.06);
}

.hero-card h3 {
  margin-top: 0;
  margin-bottom: 8px;
  font-size: 20px;
}

.hero-card p {
  margin-bottom: 0;
  line-height: 1.55;
  color: #555;
}

.homepage-carousel {
  width: 100%;
  max-width: 100%;
  margin-bottom: 25px;
}

.homepage-carousel .carousel-inner,
.homepage-carousel .item,
.homepage-carousel .item img {
  width: 100%;
  height: 380px;
}

.homepage-carousel .item img {
  object-fit: cover;
}

@media (max-width: 768px) {
  .homepage-hero {
    padding: 0 15px 20px 15px;
    margin: 0 0 20px 0;
  }

  .hero-subtitle,
  .hero-text {
    width: 100%;
    max-width: 100%;
  }

  .hero-cards {
    display: block;
    width: 100%;
  }

  .hero-card {
    width: 100%;
    max-width: 100%;
    margin-bottom: 12px;
    padding: 15px 16px;
  }

  .hero-card h3 {
    font-size: 18px;
    line-height: 1.25;
  }

  .homepage-carousel .carousel-inner,
  .homepage-carousel .item,
  .homepage-carousel .item img {
    height: 240px;
  }
}
</style>