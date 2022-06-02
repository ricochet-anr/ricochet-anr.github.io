---
title: "RICOCHET - openings"
layout: textlay
excerpt: "openings"
sitemap: false
permalink: /jobs/
---

# Open positions

We are always looking for bright and talented students to join our research group.
If you are interested in joining us, please contact one of us directly by email (see [team members](team/))

## Available PhD positions

{% for openings in site.data.jobslist %}
{% if openings.active == 1%}

<b>{{ openings.style }}</b>  au {{openings.institution}}<br/>
 <em>""{{openings.title}}"</em><br/>

 <p>
      {% if openings.pdf%} <button type="button" class="btn btn-light" onclick="window.location='/assets/jobs/{{openings.pdf}}';">PhD Subject description</button> {% endif %}
    </p>


 {% endif %}
 {% endfor %}
