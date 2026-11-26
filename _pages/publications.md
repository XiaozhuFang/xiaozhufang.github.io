---
layout: academic
title: Publications
permalink: /publications/
sections:
  - category: journal
    title: Journal papers
    id: journal-papers
  - category: conference
    title: Conference papers
    id: conference-papers
  - category: manuscript
    title: Submitted manuscripts
    id: submitted-manuscripts
---

<nav class="section-jump" aria-label="Publication categories">
  {% for section in page.sections %}
  <a href="#{{ section.id }}">{{ section.title }}</a>
  {% endfor %}
</nav>

{% for section in page.sections %}
<section class="record-section" aria-labelledby="{{ section.id }}">
  <h2 id="{{ section.id }}">{{ section.title }}</h2>
  {% assign papers = site.data.papers | where: 'category', section.category %}
  <ul class="paper-list{% if section.category == 'manuscript' %} paper-list-undated{% endif %}">
    {% for paper in papers %}
    {% include paper-row.html paper=paper %}
    {% endfor %}
  </ul>
</section>
{% endfor %}

