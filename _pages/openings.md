---
title: "RICOCHET - openings"
layout: textlay
excerpt: "openings"
sitemap: false
permalink: /jobs
---

# Open positions

We are always looking for bright and talented students to join our research group.
If you are interested in joining us, please contact one of us directly by email (see [team members](team/))

## PhD positions

{% for jobs in site.data.jobslist %}
{% if jobs.active == 1%}

<b>{{ jobs.jobstyle }}</b> ({{ressources.institution}})<br/>
 <em>{{ jobs.title }}</em><br/>

 <p>
      {% if jobs.pdf%} <button type="button" class="btn btn-light" onclick="window.location='/assets/jobs/{{jobs.pdf}}';">Slides</button> {% endif %}
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
