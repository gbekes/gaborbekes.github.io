---
title: "Research"
layout: single
author_profile: false
permalink: /research/
toc: true
toc_label: "Research Sections"
toc_icon: "bookmark"
toc_sticky: true
---


## Publications in Refereed Journals

{% for pub in site.data.publications.refereed_journals %}
<div class="research-publication">
<h3>{{ pub.title }}</h3>
<p><em>with {% for author in pub.authors %}{% unless forloop.first %}, {% endunless %}{{ author }}{% endfor %}</em></p>

<div style="background: var(--wes-light-{{ pub.journal.color }}); padding: 1rem; border-radius: 8px; margin: 1rem 0;">
  <p>{% if pub.journal.url %}<a href="{{ pub.journal.url }}" class="journal" target="_blank">{{ pub.journal.name }}</a>{% else %}<span class="journal">{{ pub.journal.name }}</span>{% endif %} {{ pub.journal.details }}</p>
</div>

{% if pub.abstract %}
<div class="abstract-section">
<strong>Abstract:</strong>
<div class="abstract-text abstract-preview" id="abstract{{ forloop.index }}Preview">
{{ pub.abstract.preview }}
</div>
<div class="abstract-text abstract-full" id="abstract{{ forloop.index }}Full">
{{ pub.abstract.full }}
</div>
<button class="abstract-toggle" onclick="toggleAbstract({{ forloop.index }})">More</button>
</div>
{% endif %}

{% if pub.links.size > 0 %}
<div class="links" style="text-align: center; background: white; padding: 1.5rem; border-radius: 8px; margin: 1rem 0; border: 2px dashed var(--wes-coral);">
{% for link in pub.links %}
{% if link.url != "[To be added]" %}
<a href="{{ link.url }}" class="btn btn--small {% if link.type == 'wp' %}btn--secondary{% elsif link.type == 'data' %}btn--data{% elsif link.type == 'blog' %}btn--info{% endif %}" {% if link.url contains 'http' %}target="_blank"{% endif %}>{{ link.label }}</a>
{% endif %}
{% endfor %}
</div>
{% endif %}

{% if pub.media.size > 0 %}
<div style="background: var(--wes-light-coral); padding: 1rem; border-radius: 8px; border-left: 4px solid var(--wes-coral);">
<strong>Media:</strong> 
{% for media in pub.media %}{% unless forloop.first %}, {% endunless %}<a href="{{ media.url }}" {% if media.url contains 'http' %}target="_blank"{% endif %}>{{ media.name }}</a>{% endfor %}
</div>
{% endif %}
</div>
{% endfor %}

## Publications beyond economics

{% assign counter = site.data.publications.refereed_journals.size %}
{% for pub in site.data.publications.publications_beyond_economics %}
{% assign counter = counter | plus: 1 %}
<div class="research-publication">
<h3>{{ pub.title }}</h3>
<p><em>with {% for author in pub.authors %}{% unless forloop.first %}, {% endunless %}{{ author }}{% endfor %}</em></p>

<div style="background: var(--wes-light-{{ pub.journal.color }}); padding: 1rem; border-radius: 8px; margin: 1rem 0;">
  <p>{% if pub.journal.url %}<a href="{{ pub.journal.url }}" class="journal" target="_blank">{{ pub.journal.name }}</a>{% else %}<span class="journal">{{ pub.journal.name }}</span>{% endif %} {{ pub.journal.details }}</p>
</div>

{% if pub.abstract %}
<div class="abstract-section">
<strong>Abstract:</strong>
<div class="abstract-text abstract-preview" id="abstract{{ counter }}Preview">
{{ pub.abstract.preview }}
</div>
<div class="abstract-text abstract-full" id="abstract{{ counter }}Full">
{{ pub.abstract.full }}
</div>
<button class="abstract-toggle" onclick="toggleAbstract({{ counter }})">More</button>
</div>
{% endif %}

{% if pub.links.size > 0 %}
<div class="links" style="text-align: center; background: white; padding: 1.5rem; border-radius: 8px; margin: 1rem 0; border: 2px dashed var(--wes-coral);">
{% for link in pub.links %}
{% if link.url != "[To be added]" %}
<a href="{{ link.url }}" class="btn btn--small {% if link.type == 'wp' %}btn--secondary{% elsif link.type == 'data' %}btn--data{% elsif link.type == 'blog' %}btn--info{% endif %}" {% if link.url contains 'http' %}target="_blank"{% endif %}>{{ link.label }}</a>
{% endif %}
{% endfor %}
</div>
{% endif %}

{% if pub.media.size > 0 %}
<div style="background: var(--wes-light-coral); padding: 1rem; border-radius: 8px; border-left: 4px solid var(--wes-coral);">
<strong>Media:</strong> 
{% for media in pub.media %}{% unless forloop.first %}, {% endunless %}<a href="{{ media.url }}" {% if media.url contains 'http' %}target="_blank"{% endif %}>{{ media.name }}</a>{% endfor %}
</div>
{% endif %}
</div>
{% endfor %}

# Work in progress

## Work in progress I: Globalization 

{% assign counter = counter | plus: site.data.publications.publications_beyond_economics.size %}
{% for pub in site.data.publications.work_in_progress_globalization %}
{% assign counter = counter | plus: 1 %}
<div class="content-section">
<h3>{{ pub.title }}</h3>
<p><em>with {% for author in pub.authors %}{% unless forloop.first %}, {% endunless %}{{ author }}{% endfor %}</em></p>

{% if pub.abstract %}
<div class="abstract-section">
<strong>Abstract:</strong>
<div class="abstract-text abstract-preview" id="abstract{{ counter }}Preview">
{{ pub.abstract.preview }}
</div>
<div class="abstract-text abstract-full" id="abstract{{ counter }}Full">
{{ pub.abstract.full }}
</div>
<button class="abstract-toggle" onclick="toggleAbstract({{ counter }})">More</button>
</div>
{% endif %}

{% if pub.links.size > 0 %}
<div class="links" style="text-align: center; background: white; padding: 1.5rem; border-radius: 8px; margin: 1rem 0; border: 2px dashed var(--wes-coral);">
{% for link in pub.links %}
{% if link.url != "[To be added]" %}
<a href="{{ link.url }}" class="btn btn--small {% if link.type == 'wp' %}btn--secondary{% elsif link.type == 'data' %}btn--data{% elsif link.type == 'blog' %}btn--info{% endif %}" {% if link.url contains 'http' %}target="_blank"{% endif %}>{{ link.label }}</a>
{% endif %}
{% endfor %}
</div>
{% endif %}
</div>
{% endfor %}

## Work in progress II: Organizations 

{% for pub in site.data.publications.work_in_progress_organizations %}
{% assign counter = counter | plus: 1 %}
<div class="content-section">
<h3>{{ pub.title }}</h3>
<p><em>with {% for author in pub.authors %}{% unless forloop.first %}, {% endunless %}{{ author }}{% endfor %}</em>{% if pub.status %}, {{ pub.status }}{% endif %}</p>

{% if pub.abstract %}
<div class="abstract-section">
<strong>Abstract:</strong>
<div class="abstract-text abstract-preview" id="abstract{{ counter }}Preview">
{{ pub.abstract.preview }}
</div>
<div class="abstract-text abstract-full" id="abstract{{ counter }}Full">
{{ pub.abstract.full }}
</div>
<button class="abstract-toggle" onclick="toggleAbstract({{ counter }})">More</button>
</div>
{% endif %}

{% if pub.links.size > 0 %}
<div class="links" style="text-align: center; background: white; padding: 1.5rem; border-radius: 8px; margin: 1rem 0; border: 2px dashed var(--wes-coral);">
{% for link in pub.links %}
{% if link.url != "[To be added]" %}
<a href="{{ link.url }}" class="btn btn--small {% if link.type == 'wp' %}btn--secondary{% elsif link.type == 'data' %}btn--data{% elsif link.type == 'blog' %}btn--info{% endif %}" {% if link.url contains 'http' %}target="_blank"{% endif %}>{{ link.label }}</a>
{% endif %}
{% endfor %}
</div>
{% endif %}
</div>
{% endfor %}

# Books, book chapters

<div class="content-section">
<p>Measuring competitiveness in Europe: resource allocation, granularity and trade (editor, with Carlo Altomonte), Bruegel, Brussels, January 2016</p>

<p>Measuring competitiveness in a granular and global world (with Carlo Altomonte) in Altomonte, C. and G. Békés (2016) Measuring competitiveness in Europe: resource allocation, granularity and trade pp 3-13</p>

<p>Micro-founded measurement of regional competitiveness in Europe (with Gianmarco I.P. Ottaviano),  in Altomonte, C. and G. Békés (2016) Measuring competitiveness in Europe: resource allocation, granularity and trade pp26-46</p>

<p>Barriers to data access and matching in Europe (with Zsuzsa Holler) in Davide Castellani and Andreas Koch "Mapping competitiveness with European, data", 2015, Bruegel Bluprint Series #23, Bruegel, Brussels</p>

<p>Still standing: how European firms weathered the crisis - (with M. Koren, B. Muraközy, L. Halpern) December 2011, Bruegel Bluprint Series #15, Bruegel, Brussels</p>

<p>Motives of corporate location choice (in Hungarian, in English), Chapter 2.1 in The Hungarian labour market, 2004 : Review and analysis / ed. by K. Fazekas, J. Koltay and Zs. Cseres-Gergely. - Bp. : MTA KTI, 2004.</p>
</div>

## Resting projects 

<div class="content-section">
<ul>
<li>Gender differences in entrepreneurial choices (with Anna May and Aniko Hannak)</li>
<li>Auto suppliers (with Balázs Muraközy)</li>
<li>Floods, amenities and house prices (with Áron Horváth and Zoltán Sápi) MTA KTI Discussion Paper 2016</li>
<li>Trade Complexity and Productivity  (with Carlo Altomonte)  CeFiG Working Papers, no. 12, October 2010 (NEW VERSION)</li>
<li>Location of manufacturing FDI in Hungary: How important are inter-company relationships?  Magyar Nemzeti Bank Working Paper, 2005 December, WP 2005/7. new version, available on request</li>
</ul>
</div>

## Non-technical posts

* Technology adoption via machine imports: Identifying who learns from peers (with Péter Harasztosi), VOXEU column, 30 September 2019
* The ladder of internationalization modes (with Balázs Muraküzy), VOXEU column, 28 March 2018
* The Knowns and Unknowns of the European Competitiveness Debate (with Carlo Altomonte ) Roubini EconoMonitor,  April 27, 2016 
* Internationalisation and innovation of firms: Give them one roof (with Altomonte, Aquilante and Ottaviano) VOXEU column , 21 March 2014
* Restarting growth - Why institutions matter for Hungarian companies, Portfolio.hu  (19 October 2012)
* Temporary trade: exporting only once in a while (with Balázs Muraközy), VOXEU column 20 September 2012
* Still Standing: Global crisis and European Firms (with Koren, Halpern, Muraközy) VOXEU column 18 May 2012
* Trading ain't easy: How complex is it to trade goods? (with Carlo Altomonte), VOXEU column(19 November 2010)
* Trade collapse during the 2009 crisis: How did European companies fare?, Presentation at seminar DG Trade of the European Commission, 2011 Budapest
* Financial crisis: from global to local, Budapest Times, Monday, 13 October 2008

## Policy reports

HUNGARY – How did exporting firms cope with the crisis? - EFIGE Country Report: Hungary, February 2011 (with Miklos Koren, Laszlo Halpern and Balázs Muraközy)

Internationalisation of corporate activity and competitiveness of the European economy: some policy implications (with Carlo Altomonte), Micro-Dyn WP 6/2011 

Agglomeration Premium and Trading Activity of Firms –A discussion, (with Peter Harasztosi), 3rd MICRO-DYN NEWSLETTER (September 2010)

Hungary and the Euro: Waitingfor Godot in Economic and Political Challenges of Acceding to the Euro area in the post-Lehman Brothers' World, Open Society Institute – Sofia /European Policies Initiative (October 2009)

# In Hungarian (Magyarul)

## Papers in Hungarian journals (Folyóirat cikkek)

Területi Egyensúly a munkaerőpiac és az ingatlanárak kapcsolata Magyarországon (with Marta Bisztray), Szigma, LI. (2020) 3. 185-214 (September 2020) 

Beszállítói termékek a magyar feldolgozóiparban ( with Balázs Muraközy), Közgazdasági Szemle LXIII. évf., 2016. október (1046—1073. o.) ,

Lakóingatlanárak és települési különbségek (with Horváth Áron , Sápi Zoltán) Közgazdasági Szemle, 63. évf. 12. sz. 2016. p. 1289-1323.

Külkereskedelem és a vállalatok közötti különbségek (with Balázs Muraközy and László Halpern) Közgazdasági Szemle 2013 Január

Magyar Gazellák. A gyors növekedésű vállalatok jellemzői és kialakulásuk elemzése (Balázs Muraközy) Közgazdasági Szemle LI X. évf., 2012. március (233—262. o.) 

A teremtő rombolás szerepe a vállalati termelékenység alakulásában Magyarországon (with László Halpern and Balázs Muraközy), Közgazdasági Szemle, vol 63. 2. szám 2011. február

Optimális valutaövezetek, gazdasági integráltság és hasonlatosság: az Európai Unió példája(Optimum currency areas, economic integration and similarity: the case of the EU) in Hungarian in Közgazdasági Szemle (1998. (Vol 45.) 7-8. . 709p)

## Hungarian Book chapters (Könyvfejezetek)

Nemzeti innovációs rendszer (National Innovation System) in  G. Pörzse (ed) Kutatásszervezés és innovációmenedzsment az egészség- és élettudományok területén, Semmelweis Kiadó, 2011

Innovációs klaszterek és tudásparkok (Innovation clusters and science parks) in Pörzse Gábor (ed): Innovációmenedzsment. - Budapest : Semmelweis Kiadó, 2008.


<script>
function toggleAbstract(id) {
    const preview = document.getElementById(`abstract${id}Preview`);
    const full = document.getElementById(`abstract${id}Full`);
    const toggle = document.querySelector(`button[onclick="toggleAbstract(${id})"]`);
    
    if (full.style.display === 'none' || full.style.display === '') {
        preview.style.display = 'none';
        full.style.display = 'block';
        toggle.textContent = 'Less';
    } else {
        preview.style.display = 'block';
        full.style.display = 'none';
        toggle.textContent = 'More';
    }
}
</script>
