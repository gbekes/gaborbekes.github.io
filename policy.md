---
title: "Policy"
layout: single
author_profile: false
permalink: /policy/
---

Short research notes for public policy, based on micro data and standard methods, with a technical
appendix. Each note has an English and a Hungarian summary.

*Rövid kutatási jegyzetek a szakpolitika számára, mikroadatok és bevett módszerek alapján, technikai
függelékkel. Minden jegyzethez angol és magyar összefoglaló tartozik.*

{% for note in site.data.policy %}
<div class="pub policy-note">
  <h3>{% if note.links.size > 0 %}<a href="{{ note.links[0].url }}">{{ note.en.title }}</a>{% else %}{{ note.en.title }}{% endif %}</h3>
  <p class="pub-meta"><em>{{ note.hu.title }}</em></p>
  <p class="pub-meta">{{ note.authors | join: ", " }} &mdash; {{ note.series }} {{ note.number }} &mdash; {{ note.date }}{% if note.status %}<span class="pub-status">{{ note.status }}</span>{% endif %}</p>
  <details class="pub-abstract"><summary>Abstract (English)</summary>
    <p>{{ note.en.abstract }}</p>
    <p><strong>Keywords:</strong> {{ note.en.keywords }}. <strong>JEL:</strong> {{ note.jel }}.</p>
  </details>
  <details class="pub-abstract" lang="hu"><summary>Összefoglaló (magyarul)</summary>
    <p>{{ note.hu.abstract }}</p>
    <p><strong>Kulcsszavak:</strong> {{ note.hu.keywords }}. <strong>JEL:</strong> {{ note.jel }}.</p>
  </details>
  {% if note.links.size > 0 %}<p class="pub-links">{% for link in note.links %}{% if link.url == "" %}<span class="btn btn--small btn--disabled">{{ link.label }}</span>{% else %}<a href="{{ link.url }}" class="btn btn--small"{% if link.url contains 'http' %} target="_blank" rel="noopener"{% endif %}>{{ link.label }}</a>{% endif %}{% endfor %}</p>{% endif %}
</div>
{% endfor %}
