---
title: All Job Descriptions
layout: page
bodyClass: page-home
---

<div class="row pt-6 pb-6">
{% assign jobs = site.data.jobs | sort: 'title'  %}
<ul style="list-style: none;">
{% for job in jobs %}
             <li><a href="/job/{{ job.slug }}"><strong>{{job.title}}</strong> at {{job.company}}</a></li>

{% endfor %}
</ul>
