---
title: "Goodwill Lab - Publications"
layout: textlay
excerpt: "Goodwill Lab -- Publications."
sitemap: false
permalink: /publications/
---
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

# Publications

{% for year in site.data.publications %}
  <h2>{{ year.text }}</h2>
{% for pub in year.elements %}

  <span style="font-weight: 500;color:crimson;">[{{ pub.conference}}]</span> {% if pub.paper-link %}
  [<a href="{{pub.paper-link}}"><i class="fa fa-file" aria-hidden="true"></i> Paper</a>] 
  {% endif %} {% if pub.code-link %}[<a href="{{pub.code-link}}"><i class="fab fa-fw fa-github" aria-hidden="true"></i>Artifact</a>]{% endif %}   {% if pub.slides-link %}[<a href="{{pub.slides-link}}"><i class="fab fa-fw fa-slideshare" aria-hidden="true"></i>Presentation</a>]{%endif%}<br/> 
<span style="font-weight: 1000">{{ pub.paper}}</span> <br/>
 <span style="font-weight: 400;color:grey;"> {{pub.authors}}</span><br/>
<!-- <em><span style="font-weight: 400;color:grey;"> {{pub.conference-name}}</span></em><br/> -->
{% endfor %}
{% endfor %}
