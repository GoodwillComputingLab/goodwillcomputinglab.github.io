---
title: "Goodwill Lab - Publications"
layout: textlay
excerpt: "Goodwill Lab -- Publications."
sitemap: false
permalink: /publications/
---

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

# Publications

<style>
.custom-label {
  background-color: #DC143C;
  color: white;
  padding: 3px 8px;
  border-radius: 8px;
  font-weight: 700;
  display: inline-block;
  font-size: 14px;
  margin-right: 10px;
}

.pub-entry {
  margin-bottom: 26px;
  padding-bottom: 20px;
  border-bottom: 1px solid #eeeeee;
  line-height: 1.45;
}

.pub-links {
  display: inline-block;
  margin-left: 2px;
}

.pub-link {
  display: inline-block;
  margin-right: 6px;
  padding: 4px 10px;
  border-radius: 999px;
  background: #f3f4f6;
  color: #4a78a8;
  text-decoration: none;
  font-size: 14px;
  font-weight: 500;
}

.pub-link:hover {
  background: #DC143C;
  color: white;
  text-decoration: none;
}

.pub-link i {
  margin-right: 3px;
}

.pub-title {
  display: block;
  margin-top: 8px;
  font-weight: 600;
  color: #2f2f2f;
  font-size: 17px;
  line-height: 1.3;
}

.pub-authors {
  display: block;
  margin-top: 5px;
  font-weight: 400;
  color: #777;
  font-size: 15px;
  line-height: 1.35;
}

/* .publication-year {
  margin-top: 38px;
  margin-bottom: 18px;
  font-size: 42px;
  font-weight: 750;
  color: #333;
} */
</style>

{% for year in site.data.publications %}

<h2>{{ year.text }}</h2>

{% for pub in year.elements %}

{% assign paper_url = pub.paper-link %}
{% assign artifact_url = pub.code-link %}
{% assign presentation_url = pub.slides-link %}

{% if artifact_url == nil or artifact_url == "" %}
{% assign artifact_url = paper_url %}
{% endif %}

{% if presentation_url == nil or presentation_url == "" %}
{% assign presentation_url = paper_url %}
{% endif %}

<div class="pub-entry" markdown="0">
<span class="custom-label">{{ pub.conference }}</span>
<span class="pub-links"><a href="{{ paper_url }}" class="pub-link" target="_blank"><i class="fa fa-file" aria-hidden="true"></i>Paper</a><a href="{{ artifact_url }}" class="pub-link" target="_blank"><i class="fab fa-fw fa-github" aria-hidden="true"></i>Artifact</a><a href="{{ presentation_url }}" class="pub-link" target="_blank"><i class="fab fa-fw fa-slideshare" aria-hidden="true"></i>Presentation</a></span>
<span class="pub-title">{{ pub.paper }}</span>
<span class="pub-authors">{{ pub.authors }}</span>
</div>

{% endfor %}
{% endfor %}