---
layout: default
title: Home
---

<section id="bio" class="section bio-header">
  <img class="bio-photo" src="{{ '/assets/img/bin-peng.jpg' | relative_url }}" alt="Portrait of {{ site.author.name }}">
  <div>
  <h1>{{ site.author.name }}, PhD</h1>
  <p class="role">{{ site.author.role }}</p>
  <p class="role"><a href="{{ site.author.department_url }}">Department of Crop Sciences</a></p>
  {% for affiliation in site.author.affiliations %}
  <p class="role"><a href="{{ affiliation.url }}">{{ affiliation.name }}</a></p>
  {% endfor %}
  <p class="role"><a href="{{ site.author.university_url }}">University of Illinois Urbana-Champaign</a></p>
  <p class="contact">Email: <a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a></p>
  <p class="contact">Office: {{ site.author.office }}</p>
  </div>
</section>

<section class="section">
  <p>I am a tenure-track Assistant Professor leading the <a href="{{ site.waci_lab_url }}">Water, Agriculture, and Conservation Innovation (WACI) Lab</a> at the Department of Crop Sciences, University of Illinois Urbana-Champaign (UIUC). My core research interests center around unraveling the complexities of water, nutrient, and carbon cycles within diverse agricultural landscapes and their interconnectedness with agricultural productivity and environmental sustainability. To tackle these challenges, my research leverages various tools and methods, including field and lab measurement, computational and process-based modeling (hydrological, cropping system, ecosystem and earth system modeling), remote sensing, geospatial big data, model-data integration, and artificial intelligence.</p>

  <p>I am deeply motivated to drive transdisciplinary, convergence, and use-inspired research for breaking new ground in sustaining agricultural production and environmental quality. I am passionate about developing innovative technologies and systems solutions to foster sustainable agri-food systems and preserve a healthy environment amidst the pressures of intensifying land use and increasing weather variability. The driving force behind my research pursuits lies in addressing critical societal issues, including ensuring water, food, and energy security, enhancing water quality and environmental sustainability, and nurturing rural economies and human well-being both in the United States and across the globe.</p>

  <p>I am recruiting multiple self-motivated and enthusiastic postdoctoral researchers and graduate students. See the <a href="{{ '/hiring/' | relative_url }}">Hiring</a> page and the <a href="{{ site.waci_lab_url }}">WACI Lab site</a> for current openings.</p>
</section>

<section id="interests" class="section">
  <h2>Research Interests</h2>
  <ul class="tag-list">
    <li>Hydrology</li>
    <li>Water Quality</li>
    <li>Biogeochemistry</li>
    <li>Sustainable Agriculture</li>
    <li>Soil-Water-Nutrient Conservation</li>
    <li>Cropping System Modeling</li>
    <li>Agroecosystem Modeling</li>
    <li>Hydrological Modeling</li>
    <li>Remote Sensing</li>
    <li>Digital Agriculture</li>
    <li>Precision Conservation</li>
    <li>AI for Science</li>
    <li>Environmental Data Science</li>
  </ul>
</section>
