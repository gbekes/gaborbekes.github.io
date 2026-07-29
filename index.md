---
title: "Gábor Békés"
layout: single
author_profile: true
classes: wide
permalink: /
---

<p class="eyebrow">Vienna &middot; Budapest &mdash; Economics &amp; Data Analysis</p>

<p>Gábor Békés is associate professor of Economics at the <span class="institution-name">Central European University</span> in Vienna, senior research fellow at the <span class="institution-name">HUN-REN KRTK Institute of Economics</span> (Hungary), and research fellow at <span class="institution-name">CEPR</span> and <span class="institution-name">Centro LdA</span> (Italy). He is an applied economist who studies how globalization reshapes firms, locations, and organizations, based on large-scale firm- and transaction-level microdata. He is the co-author of <em>Data Analysis for Business, Economics, and Policy</em>, a textbook published by Cambridge University Press, and an advising fellow at the <span class="institution-name">Microsoft AI Economy Institute</span>. His <span class="institution-name">Data Analysis and AI Lab</span> supports research, produces education materials, and helps link academia and industry.</p>

<p>
  <a href="/assets/pdf/CV_BekesGabor.pdf" class="btn btn--primary" target="_blank" rel="noopener">Download CV</a>
  <a href="/research/" class="btn">Research</a>
  <a href="mailto:bekesg@ceu.edu" class="btn">Email</a>
</p>

<div class="content-section">
  <h2>What's new</h2>
  <ul class="news-list">
    {% for item in site.data.news limit: 5 %}
    <li>
      <span class="news-date">{{ item.date }}</span>
      <span class="news-body"><span class="news-tag">{{ item.tag }}</span> {{ item.text | markdownify | remove: '<p>' | remove: '</p>' }}</span>
    </li>
    {% endfor %}
  </ul>
</div>

<div class="content-section">
  <h2>Research areas</h2>
  <div class="quiet-grid">
    <div class="quiet-card">
      <h3><a href="/research/#publications-in-refereed-journals">International economics</a></h3>
      <p>Firm performance, trade, and multinational activity.</p>
      <a href="/research/#publications-in-refereed-journals" class="quiet-link">Publications &rarr;</a>
    </div>
    <div class="quiet-card">
      <h3><a href="/research/#publications-in-refereed-journals">Organizations</a></h3>
      <p>Collaboration, bias, and team performance &mdash; often measured with football data.</p>
      <a href="/research/#publications-in-refereed-journals" class="quiet-link">Publications &rarr;</a>
    </div>
    <div class="quiet-card">
      <h3><a href="/research/#publications-in-refereed-journals">Economic geography</a></h3>
      <p>Agglomeration, location choice, and firms in space.</p>
      <a href="/research/#publications-in-refereed-journals" class="quiet-link">Publications &rarr;</a>
    </div>
    <div class="quiet-card">
      <h3><a href="/research/#publications-beyond-economics">Beyond economics</a></h3>
      <p>Health research: arthritis and comorbidities.</p>
      <a href="/research/#publications-beyond-economics" class="quiet-link">Publications &rarr;</a>
    </div>
  </div>
</div>

<div class="content-section">
  <h2>Textbook</h2>
  <p><em>Data Analysis for Business, Economics, and Policy</em> (with Gábor Kézdi), Cambridge University Press, 2021. Used in courses in more than 40 countries.</p>
  <p>
    <a href="https://gabors-data-analysis.com" class="btn" target="_blank" rel="noopener">Textbook site</a>
    <a href="/textbook/" class="btn btn--info">About the book</a>
  </p>
</div>

<div class="content-section">
  <h2>Teaching</h2>
  <div class="quiet-grid">
    <div class="quiet-card">
      <h3>Data Analysis 1&ndash;4</h3>
      <p>A graduate course sequence at CEU based on the textbook.</p>
      <a href="/teaching/" class="quiet-link">Courses &rarr;</a>
    </div>
    <div class="quiet-card">
      <h3>Data Analysis with AI</h3>
      <p>Open-access upskilling course for economics and social science students.</p>
      <a href="https://gabors-data-analysis.com/ai-course/" class="quiet-link" target="_blank" rel="noopener">Course material &rarr;</a>
    </div>
  </div>
</div>

<div class="content-section">
  <h2>Recent talks</h2>
  <ul class="talks-list">
    <li><span class="year-style">2025</span> &mdash; <strong>Integrators and robot adoption</strong>, GEN Workshop. <a href="/assets/pdf/BBCG-Jul2025-slides.pdf" target="_blank" rel="noopener">Slides</a></li>
    <li><span class="year-style">Oct 2</span> &mdash; <strong>Vibe coding kills OSS</strong>, Ericsson, Automattic. <a href="https://cepr.org/publications/dp21145" target="_blank" rel="noopener">CEPR DP</a></li>
  </ul>
</div>

<div class="content-section">
  <h2>Press &amp; interviews</h2>
  <p>Featured in the Boston Globe, Financial Times, Der Standard, and Portfolio.</p>
  <p><a href="/popular-press/" class="btn btn--small">All coverage</a></p>
</div>
