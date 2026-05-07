---
title: "Goodwill Lab - Join Us"
layout: gridlay
excerpt: "Goodwill Lab: Join Us"
sitemap: false
permalink: /join/
---

# Join Us

<div class="join-page" markdown="0">

  <div class="join-hero">
    <div class="join-hero-text">
      <p class="join-kicker">Opportunities</p>

      <h2>Work with us on future computing systems.</h2>

      <p>
        The Goodwill Lab welcomes motivated students and researchers interested in
        high-performance computing, quantum computing, systems, sustainability,
        and open-source research.
      </p>

      <a class="join-button" href="mailto:d.tiwari@northeastern.edu">
        Contact us
      </a>

      <p class="join-email">d.tiwari@northeastern.edu</p>
    </div>

    <div class="join-hero-image">
      <img src="{{ site.url }}{{ site.baseurl }}/images/wantu.jpg"
           alt="Quantum computer recruitment graphic">
    </div>
  </div>

  <div class="join-info-grid">
    <div class="join-info-card">
      <h3>Prospective PhD students</h3>
      <p>
        If you want me to reply to your emails regarding doing a PhD with me,
        please mention the first two words of the title of our USENIX FAST 2013
        paper in the subject line of your email.
      </p>
      <p>
        The first line of your email should state the name of the technique
        discussed in our DSN 2015 paper.
      </p>
    </div>
  </div>

</div>

<style>
.join-page {
  max-width: 1050px;
}

.join-hero {
  display: flex;
  align-items: center;
  gap: 32px;
  padding: 10px 0 24px 0;
  border-bottom: 1px solid #e5e7eb;
}

.join-hero-text {
  flex: 1.2;
}

.join-kicker {
  color: #c8102e;
  font-weight: 700;
  letter-spacing: 0.04em;
  text-transform: uppercase;
  margin-bottom: 10px;
}

.join-hero-text h2 {
  margin-top: 0;
  margin-bottom: 18px;
  max-width: 680px;
}

.join-hero-text p {
  line-height: 1.65;
  max-width: 760px;
}

.join-button {
  display: inline-block;
  margin-top: 12px;
  padding: 10px 20px;
  background: #c8102e;
  color: white;
  border-radius: 999px;
  font-weight: 700;
  text-decoration: none;
}

.join-button:hover {
  color: white;
  text-decoration: none;
  background: #a70d25;
}

.join-email {
  margin-top: 14px;
  font-weight: 700;
  color: #444;
}

.join-hero-image {
  flex: 0.8;
  text-align: center;
}

.join-hero-image img {
  max-width: 360px;
  width: 100%;
  height: auto;
  border-radius: 0 !important;
  clip-path: none !important;
  box-shadow: 0 8px 22px rgba(0,0,0,0.08);
}

.join-info-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 22px;
  margin-top: 26px;
}

.join-info-card {
  border-left: 4px solid #c8102e;
  background: #fafafa;
  padding: 22px 24px;
  border-radius: 10px;
}

.join-info-card h3 {
  margin-top: 0;
  margin-bottom: 12px;
}

.join-info-card p {
  line-height: 1.6;
}

@media (max-width: 768px) {
  .join-hero {
    flex-direction: column;
    align-items: flex-start;
    gap: 22px;
    padding: 6px 0 22px 0;
  }

  .join-hero-image {
    width: 100%;
  }

  .join-hero-image img {
    max-width: 100%;
  }

  .join-info-card {
    padding: 18px 20px;
  }
}
</style>