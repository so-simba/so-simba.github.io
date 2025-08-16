---
layout: page
title: Work Packages
permalink: /work/
---

<div class="workpackages-grid">
  {% for wp in site.data.workpackages %}
    {% include wp-card.html wp=wp %}
  {% endfor %}
</div>
