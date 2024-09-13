---
title: "Goodwill Lab - Group members"
layout: gridlay
excerpt: "Goodwill Lab: Group members"
sitemap: false
permalink: /members/
---

# Group Members

### Director
<style>
.offset-half {
  margin-left:5%; /* 1/12 of the column width (Bootstrap’s 12-column grid) */
}
</style>

<div class="row">
<div class="col-sm-5 offset-half clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ site.data.team_members.pi.photo }}" class="img-responsive" style="float: left; border-radius: 50%; height: 100px; width: 100px; object-fit: cover; overflow: hidden;" />

  <h4>{{ site.data.team_members.pi.name }}</h4>
  
  <i>{{ site.data.team_members.pi.email }}</i>
</div>
</div>

{% for student_group in site.data.team_members.student_categories %}

  <h3>{{ student_group.text }}</h3>

{% assign number_printed = 0 %}
{% for member in student_group.individuals %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}

  <div class="row">
  {% endif %}
  <div class="col-sm-5 offset-half clearfix">
  <div style="display: flex; align-items: center;">
  {% if member.photo == nil %}
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/bio-photo.jpg" class="img-responsive" style="float: left; border-radius: 50%; height: 100px; width: 100px; object-fit: cover; overflow: hidden;" />  
  {% else %}
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" style="float: left; border-radius: 50%; height: 100px; width: 100px; object-fit: cover; overflow: hidden; image-rendering: -webkit-optimize-contrast;" />

{% endif %}
 <div style=" text-align: left; flex: 1;">
   <a href="mailto:{{ member.email }}" style="color: blue;">{{ member.name }}</a><br/>
    <a href="{{ member.webpage }}" style="color: blue;">Home Page</a><br/>
  <i>{{member.position}}</i>
  </div>
  </div>
  </div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}

  </div>
  {% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}

</div>
{% endif %}
{% endfor %}

### Goodwill Lab Friends

<div class="row">

<div class="col-sm-5 offset-half  clearfix">
{% for member in site.data.team_members.friends %}
<b>{{ member.name }}</b>, {{member.info}}
{% endfor %}
</div>

</div>
