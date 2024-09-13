---
title: "Goodwill Lab - Publications"
layout: textlay
excerpt: "Goodwill Lab -- Publications."
sitemap: false
permalink: /publications/
---
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

# Publications
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Custom Label</title>
    <style>
        .custom-label {
            background-color: #DC143C; /* Replace with your desired color */
            color: white; /* Text color */
            padding: 1px 3px; /* Space inside the label */
            border-radius: 5px; /* Rounded corners */
            font-weight: bold; /* Bold text */
            display: inline-block; /* Keeps the label inline */
            font-size:16px;
        }
    </style>
</head>

{% for year in site.data.publications %}
  <h2>{{ year.text }}</h2>
{% for pub in year.elements %}
 <span class="custom-label" style="font-weight:600">{{ pub.conference}}</span> {% if pub.paper-link %}[<a href="{{pub.paper-link}}"><i class="fa fa-file" aria-hidden="true"></i> Paper</a>]{% endif %} {% if pub.code-link %}[<a href="{{pub.code-link}}"><i class="fab fa-fw fa-github" aria-hidden="true"></i>Artifact</a>]{% endif %}{% if pub.slides-link %}[<a href="{{pub.slides-link}}"><i class="fab fa-fw fa-slideshare" aria-hidden="true"></i>Presentation</a>]{%endif%}<br/> 
<span style="font-weight: 600">{{ pub.paper}}</span> <br/>
 <span style="font-weight: 400;color:#C0C0C0;"> {{pub.authors}}</span><br/>
<!-- <em><span style="font-weight: 400;color:grey;"> {{pub.conference-name}}</span></em><br/> -->
{% endfor %}
{% endfor %}
