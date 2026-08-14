---
layout: default
title: Publications
permalink: /publications/
---

# Publications

{% assign total = site.data.publications | size %}
{% assign scholar = site.social | where: "name", "Google Scholar" | first %}

<p>{{ total }} journal publications, listed in reverse chronological order.</p>

<p class="pub-legend">* Corresponding author &middot; &dagger; Equal contribution &middot; <span class="lab-member">bold italic underline</span> indicates group members supervised by Dr. Peng &middot; Citation count and Dr. Peng's full publication record are on <a href="{{ scholar.url }}">Google Scholar</a>.</p>

{% assign remaining = total %}
{% assign by_year = site.data.publications | group_by: "year" | sort: "name" | reverse %}
{% for group in by_year %}
{% assign group_count = group.items.size %}
<h2>{{ group.name }}</h2>
<ol reversed start="{{ remaining }}" class="pub-list">
  {% for pub in group.items %}
    {% include pub-entry.html pub=pub %}
  {% endfor %}
</ol>
{% assign remaining = remaining | minus: group_count %}
{% endfor %}
