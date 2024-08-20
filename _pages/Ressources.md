---
title: "RICOCHET - ressources"
layout: textlay
excerpt: "Ressources"
sitemap: false
permalink: /ressources/
---

# Ressources

On this page you can find various material, including presentations of member of Ricochet in seminars, conferences or Ricochet meetings.

## Eusipco 2024 tutorial on bivariate signal processing

During [Eusipco 2024](https://eusipcolyon.sciencesconf.org/) in Lyon, France, we are organizing a tutorial on the basics of bivariate signal processing, focusing on polarization, physical, and quaternion viewpoints. 
Check out the [dedicated GitHub repo](https://github.com/ricochet-anr/2024_eusipco_tutorial_bivariate_signal_processing) for more details (slides, notebooks, and references).


{% include repository/repo.html repository='ricochet-anr/2024_eusipco_tutorial_bivariate_signal_processing' %}


## Presentations

{% for ressources in site.data.ressourceslist %}
{% if ressources.active == 1%}

  <b>{{ ressources.speaker }}</b> ({{ressources.institution}})<br/>
  {{ressources.date}}<br/>
   <em>{{ ressources.title }}</em><br/>

<p>
     {% if ressources.pdf%} <button type="button" class="btn btn-light" onclick="window.location='/assets/pdf/{{ressources.pdf}}';">Slides</button> {% endif %}
   </p>

<!--
<div class="collapse" id="collapse-up-{{forloop.index}}">
  <div class="card card-body">
  {{seminar.abstract}}
  </div>
</div>
-->
{% endif %}
{% endfor %}
