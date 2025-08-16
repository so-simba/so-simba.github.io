---
layout: page
title: Work Packages
permalink: /work/
---

<!-- Workflow figure -->

<div style="text-align:center; margin-top: 1.5rem; margin-bottom: 1.5rem;">
  <img src="/assets/img/SO-SIMBA_WorkLogic_webpage.png" 
       style="max-width:100%; height:auto; border-radius:4px;">
</div>

<div class="workpackages-grid">
  {% for wp in site.data.workpackages %}
    {% include wp-card.html wp=wp %}
  {% endfor %}
</div>
