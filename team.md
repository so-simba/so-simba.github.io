---
layout: page
title: Team
permalink: /team/
---

## Leads
- **Project Lead:** <Name>, <Affiliation> — Satellite remote sensing
- **Co‑Lead:** <Name>, <Affiliation> — Modeling & assimilation

## Team
- **<Name>**, <Affiliation> — Sea‑ice drift (SAR)
- **<Name>**, <Affiliation> — Freeboard (GNSS‑R)
- **<Name>**, <Affiliation> — Altimetry & tides
- **<Name>**, <Affiliation> — Data management & QA/QC

<div class="partners-grid">
{% for partner in site.data.partners %}
  {% include partner-card.html partner=partner %}
{% endfor %}
</div>
