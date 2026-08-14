---
layout: default
title: Experience
permalink: /experience/
---

# Experience

<section class="section">
  <h2>Professional Experience</h2>
  <ul class="timeline">
  {% for job in site.data.experience %}
    <li class="timeline-item">
      <div class="timeline-dates">
        {{ job.date_start }} &ndash; {% if job.date_end == "" %}present{% else %}{{ job.date_end }}{% endif %}
      </div>
      <div class="timeline-body">
        <strong>{{ job.title }}</strong><br>
        <a href="{{ job.organization_url }}">{{ job.organization }}</a>, {{ job.location }}
      </div>
    </li>
  {% endfor %}
  </ul>
</section>

<section class="section">
  <h2>Education</h2>
  <ul class="timeline">
  {% for edu in site.data.education %}
    <li class="timeline-item">
      <div class="timeline-dates">{{ edu.date_end }}</div>
      <div class="timeline-body">
        <strong>{{ edu.degree }}</strong><br>
        <a href="{{ edu.organization_url }}">{{ edu.organization }}</a>
      </div>
    </li>
  {% endfor %}
  </ul>
</section>

<section class="section">
  <h2>Honors &amp; Awards</h2>
  <ul class="timeline">
  {% for honor in site.data.honors %}
    <li class="timeline-item">
      <div class="timeline-dates">{{ honor.year }}</div>
      <div class="timeline-body">{{ honor.title }}</div>
    </li>
  {% endfor %}
  </ul>
</section>
