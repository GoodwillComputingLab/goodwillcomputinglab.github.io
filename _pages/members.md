---
title: "Goodwill Lab - Group members"
layout: gridlay
excerpt: "Goodwill Lab: Group members"
sitemap: false
permalink: /members/
---

# Group Members

<style>
.members-heading {
  margin-top: 34px;
  margin-bottom: 22px;
  font-weight: 700;
  color: #333;
}

.director-card {
  max-width: 760px;
  margin: 18px 0 46px 0;
  padding: 22px 26px;
  display: flex;
  align-items: center;
  gap: 28px;
  border-radius: 20px;
  background: #fafafa;
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.08);
}

.member-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(280px, 1fr));
  column-gap: 80px;
  row-gap: 34px;
  margin-bottom: 46px;
}

.member-card {
  padding: 16px 18px;
  display: flex;
  align-items: center;
  gap: 22px;
  border-radius: 18px;
  background: #fff;
  transition: 0.2s ease;
}

.member-card:hover {
  background: #fafafa;
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.07);
}

.member-photo {
  width: 112px;
  height: 112px;
  flex: 0 0 112px;
  border-radius: 50%;
  object-fit: cover;
  object-position: center;
  box-shadow: 0 5px 14px rgba(0, 0, 0, 0.16);
  background: #eee;
}

.member-info {
  text-align: left;
  line-height: 1.35;
}

.member-name {
  display: inline-block;
  margin-bottom: 4px;
  font-size: 20px;
  font-weight: 650;
  color: #333;
  text-decoration: none;
}

.member-name:hover {
  color: #c8102e;
  text-decoration: none;
}

.member-link {
  display: inline-block;
  margin-top: 3px;
  font-size: 16px;
  color: #666;
  text-decoration: none;
}

.member-link:hover {
  color: #c8102e;
  text-decoration: none;
}

.member-position {
  display: block;
  margin-top: 5px;
  font-size: 15px;
  color: #666;
}

.friends-card {
  max-width: 760px;
  margin: 18px 0 40px 0;
  padding: 18px 22px;
  border-radius: 18px;
  background: #fafafa;
  line-height: 1.6;
}

@media (max-width: 768px) {
  .member-grid {
    grid-template-columns: 1fr;
    row-gap: 22px;
  }

  .director-card,
  .member-card {
    gap: 18px;
  }

  .member-photo {
    width: 96px;
    height: 96px;
    flex-basis: 96px;
  }

  .member-name {
    font-size: 18px;
  }
}
</style>

<h3 class="members-heading">Director</h3>

<div class="director-card" markdown="0">
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ site.data.team_members.pi.photo }}" class="member-photo" alt="{{ site.data.team_members.pi.name }}">
<div class="member-info">
<div class="member-name">{{ site.data.team_members.pi.name }}</div>
<i class="member-position">{{ site.data.team_members.pi.email }}</i>
</div>
</div>

{% for student_group in site.data.team_members.student_categories %}

<h3 class="members-heading">{{ student_group.text }}</h3>

<div class="member-grid" markdown="0">

{% for member in student_group.individuals %}

<div class="member-card">
{% if member.photo == nil %}
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/bio-photo.jpg" class="member-photo" alt="{{ member.name }}">
{% else %}
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="member-photo" alt="{{ member.name }}">
{% endif %}
<div class="member-info">
<a href="mailto:{{ member.email }}" class="member-name">{{ member.name }}</a><br>
{% if member.webpage %}
<a href="{{ member.webpage }}" class="member-link">Home Page</a>
{% endif %}
<i class="member-position">{{ member.position }}</i>
</div>
</div>

{% endfor %}

</div>

{% endfor %}

<h3 class="members-heading">Goodwill Lab Friends</h3>

<div class="friends-card" markdown="0">
{% for member in site.data.team_members.friends %}
<p><b>{{ member.name }}</b> {{ member.info }}</p>
{% endfor %}
</div>