---
title: UX Jobs by Role
layout: page
bodyClass: page-home
---

<div class="row pt-6 pb-6">
{% assign groups = site.data.jobs | group_by: "role" | sort: 'name'  %}
{% for g in groups %}
 <div class="col-12 col-md-6 mb-3">
     <div class="team team-summary">
         <div class="team-meta">
             <h2 class="team-name"><a href="/role/{{ g.items[0].role_slug }}">{{g.name}}</a> <span class="badge rounded-pill bg-secondary">{{g.items.size}}</span></h2>
         </div>
     </div>
 </div>
{% endfor %}
</div>
