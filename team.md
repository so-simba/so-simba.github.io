---
layout: page
title: Team
permalink: /team/
---

The SO-SIMBA team brings together researchers in satellite remote sensing, oceanography, and climate science from across Europe and Canada, combining strengths in spaceborne observations, field measurements, and modelling. 

<div class="partners-grid">
{% for partner in site.data.partners %}
  {% include partner-card.html partner=partner %}
{% endfor %}
</div>
