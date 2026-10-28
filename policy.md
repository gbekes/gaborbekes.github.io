---
title: "Policy"
layout: single
author_profile: false
permalink: /policy/
---

Research for public policy, by topic: short research notes based on micro data and standard
methods, with a technical appendix, one-page executive summaries in English and Hungarian, and
where the work has been cited.

*Szakpolitikai kutatások témák szerint: rövid kutatási jegyzetek mikroadatok és bevett módszerek
alapján, technikai függelékkel, egyoldalas vezetői összefoglalók angolul és magyarul, és hol
hivatkoztak a munkára.*

<p class="jumplinks">{% for topic in site.data.policy %}<a href="#{{ topic.id }}">{{ topic.title | split: ":" | first }}</a>{% endfor %}</p>

{% for topic in site.data.policy %}
<section class="policy-topic" id="{{ topic.id }}">
<h2>{{ topic.title }}</h2>
{% if topic.title_hu %}<p class="pub-meta"><em>{{ topic.title_hu }}</em></p>{% endif %}
{% if topic.intro %}<p class="policy-intro">{{ topic.intro }}</p>{% endif %}
{% if topic.intro_hu %}<p class="policy-intro" lang="hu"><em>{{ topic.intro_hu }}</em></p>{% endif %}
{% if topic.coming %}<p class="policy-coming"><span class="pub-status">{{ topic.coming }}</span>{% if topic.coming_hu %} <span class="pub-status" lang="hu">{{ topic.coming_hu }}</span>{% endif %}</p>{% endif %}

{% for note in topic.notes %}
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

{% if topic.summaries.size > 0 %}
<div class="pub-media policy-block">
  <span class="pub-label">Executive summary &middot; Vezetői összefoglaló</span>
  <p class="pub-links">{% for s in topic.summaries %}<a href="{{ s.url }}" class="btn btn--small">{{ s.label }}</a>{% endfor %}</p>
</div>
{% endif %}

{% if topic.cited_in.size > 0 %}
<div class="pub-media policy-block policy-cited">
  <span class="pub-label">Cited in &middot; Hivatkozások</span>
  <ul>
  {% for c in topic.cited_in %}<li><a href="{{ c.url }}" target="_blank" rel="noopener"><em>{{ c.title }}</em></a>{% if c.title_en %} ({{ c.title_en }}){% endif %}. {{ c.issuer }}, {{ c.date }}{% if c.where %}, {{ c.where }}{% endif %}.{% if c.note %} {{ c.note }}{% endif %}</li>{% endfor %}
  </ul>
</div>
{% endif %}
</section>
{% endfor %}
