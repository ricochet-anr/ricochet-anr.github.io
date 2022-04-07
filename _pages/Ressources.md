---
title: "RICOCHET - ressources"
layout: textlay
excerpt: "Ressources"
sitemap: false
permalink: /ressources/
---

# Ressources

On this page you can find various material, including presentations of member of Ricochet in seminars, conferences or Ricochet meetings.


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
