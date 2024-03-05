---
title: "RICOCHET  - Team"
layout: gridlay
excerpt: "RICOCHET: Team members"
sitemap: false
permalink: /team/
---

# Project Members

 **We are  looking for new PhD students, Postdocs, and Master students to join the project team** [(see openings)]({{ site.url }}{{ site.baseurl }}/jobs) **!**

## Faculty
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} </i> <!--<br>email: <{{ member.email }}></i> -->
    <br/>
  {{member.lab}}
  <br/>
  <b>{{member.keywords}}</b>
  <br/>
  <ul class="list-inline">
  {% if member.email %}
  <li class="list-inline-item">
  <a href="{{member.email}}"  title="email" class="no-mark-external">
    <span class="fa fa-envelope"></span>
    <!-- <span class="sr-only">{{ name }}</span> -->
  </a>
  </li>
  {% endif %}
  {% if member.website %}
  <li class="list-inline-item">
  <a href="{{member.website}}" title="personal website" class="no-mark-external">
    <span class="fa fa-globe"></span>
    <!-- <span class="sr-only">{{ name }}</span> -->
  </a>
  </li>
  {% endif %}
  {% if member.scholar %}
  <li class="list-inline-item">
  <a href="{{member.scholar}}" title="scholar" class="no-mark-external">
    <span class="ai ai-lg ai-google-scholar-square"></span>
    <!-- <span class="sr-only">{{ name }}</span> -->
  </a>
  </li>
  {% endif %}
  {% if member.researchgate %}
  <li class="list-inline-item">
  <a href="{{member.researchgate}}" title="rg" class="no-mark-external">
    <span class="ai ai-lg ai-researchgate-square"></span>
    <!-- <span class="sr-only">{{ name }}</span> -->
  </a>
  </li>
  {% endif %}
  </ul>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
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




## Post-doctoral researchers
{% assign number_printed = 0 %}
{% for member in site.data.postdocs %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} </i> <!--<br>email: <{{ member.email }}></i> -->
    <br/>
  <p class="text-muted"> {{member.subject}}</p>
  <ul class="list-inline">
  {% if member.email %}
  <li class="list-inline-item">
  <a href="mailto:firstname.lastname@univ-lorraine.fr"  title="email" class="no-mark-external">
    <span class="fa fa-envelope"></span>
    <!-- <span class="sr-only">{{ name }}</span> -->
  </a>
  </li>
  {% endif %}
  {% if member.website %}
  <li class="list-inline-item">
  <a href="{{member.website}}" title="personal website" class="no-mark-external">
    <span class="fa fa-globe"></span>
    <!-- <span class="sr-only">{{ name }}</span> -->
  </a>
  </li>
  {% endif %}
  {% if member.scholar %}
  <li class="list-inline-item">
  <a href="{{member.scholar}}" title="scholar" class="no-mark-external">
    <span class="ai ai-lg ai-google-scholar-square"></span>
    <!-- <span class="sr-only">{{ name }}</span> -->
  </a>
  </li>
  {% endif %}
  {% if member.researchgate %}
  <li class="list-inline-item">
  <a href="{{member.researchgate}}" title="rg" class="no-mark-external">
    <span class="ai ai-lg ai-researchgate-square"></span>
    <!-- <span class="sr-only">{{ name }}</span> -->
  </a>
  </li>
  {% endif %}
  </ul>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
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




<!-- {% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.duration }} <br> Role: {{ member.info }}</i>
  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %} -->

## Alumni
{% assign number_printed = 0 %}
{% for member in site.data.alumni_postdocs %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} </i> <!--<br>email: <{{ member.email }}></i> -->
    <br/>
  <p class="text-muted"> {{member.subject}}</p>
  <ul class="list-inline">
  {% if member.email %}
  <li class="list-inline-item">
  <a href="mailto:firstname.lastname@univ-lorraine.fr"  title="email" class="no-mark-external">
    <span class="fa fa-envelope"></span>
    <!-- <span class="sr-only">{{ name }}</span> -->
  </a>
  </li>
  {% endif %}
  {% if member.website %}
  <li class="list-inline-item">
  <a href="{{member.website}}" title="personal website" class="no-mark-external">
    <span class="fa fa-globe"></span>
    <!-- <span class="sr-only">{{ name }}</span> -->
  </a>
  </li>
  {% endif %}
  {% if member.scholar %}
  <li class="list-inline-item">
  <a href="{{member.scholar}}" title="scholar" class="no-mark-external">
    <span class="ai ai-lg ai-google-scholar-square"></span>
    <!-- <span class="sr-only">{{ name }}</span> -->
  </a>
  </li>
  {% endif %}
  {% if member.researchgate %}
  <li class="list-inline-item">
  <a href="{{member.researchgate}}" title="rg" class="no-mark-external">
    <span class="ai ai-lg ai-researchgate-square"></span>
    <!-- <span class="sr-only">{{ name }}</span> -->
  </a>
  </li>
  {% endif %}
  </ul>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
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

