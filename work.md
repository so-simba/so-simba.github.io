---
layout: page
title: Work Packages
permalink: /work/
---

<!-- Workflow figure -->
<p align="center">
  <img src="{{ '/assets/img/SO-SIMBA_WorkLogic_webpage' | relative_url }}" alt="SO-SIMBA Workflow" style="max-width:100%;height:auto;border-radius:4px;">
</p>

<div class="workpackages-grid">
  {% for wp in site.data.workpackages %}
    {% include wp-card.html wp=wp %}
  {% endfor %}
</div>
