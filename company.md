---
title: UX Jobs by Company
layout: page
bodyClass: page-home
---

<div class="row pt-6 pb-6">
{% assign groups = site.data.jobs | group_by: "company" | sort: 'name'  %}
{% for g in groups %}
 <div class="col-12 col-md-4 mb-3">
     <div class="team team-summary">
         <div class="team-meta">
             <h2 class="team-name"><a href="/company/{{ g.name }}">{{g.name}}</a> <span class="badge rounded-pill bg-secondary">{{g.items.size}}</span></h2>
         </div>
     </div>
 </div>
{% endfor %}
</div>
