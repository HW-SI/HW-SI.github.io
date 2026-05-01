---
permalink: /
title: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<div class="site-hero">
  <p class="site-eyebrow">High-energy astrophysics | Markoff group | University of Amsterdam</p>
  <h1>Haowen Si</h1>
  <p class="site-lead">Master's student in Astrophysics working on black-hole jet modeling, high-energy cosmic rays, neutrinos, and multi-messenger signatures from compact-object systems.</p>
  <div class="site-actions">
    <a class="btn" href="/research/">Research</a>
    <a class="btn" href="/blog/">Blog</a>
    <a class="btn" href="https://seramarkoff.com" target="_blank" rel="noopener">Group</a>
  </div>
</div>

<section class="site-section">
  <h2>Research Focus</h2>
  <p>My current focus is on <strong>microquasars</strong>, stellar-mass black holes with relativistic jets, using nearby sources such as <strong>V4641 Sgr</strong> as time-resolvable laboratories for jet physics. The core questions are how particles are accelerated in jets and how jets couple to their surrounding medium, shaping the gamma-ray and neutrino emission we can detect.</p>

  <div class="site-grid">
    <article class="site-card">
      <h3>Microquasar Jets</h3>
      <p>Nearby stellar-mass black-hole systems provide laboratories for testing jet acceleration and emission models.</p>
    </article>
    <article class="site-card">
      <h3>Multi-messenger Modeling</h3>
      <p>Jet models are connected to gamma-ray and neutrino predictions through detector-space forecasts.</p>
    </article>
    <article class="site-card">
      <h3>Jet-Medium Coupling</h3>
      <p>Interaction regions, shocks, and particle transport link the source physics to the surrounding Galactic environment.</p>
    </article>
  </div>
</section>

<section class="site-section">
  <h2>Current Project</h2>
  <p>I am building an end-to-end pipeline that connects:</p>
  <ul class="site-list">
    <li><strong>Jet emission models (BHJet/HADJet)</strong> to predict lepto-hadronic particle populations and radiation;</li>
    <li><strong>Jet termination and interaction regions</strong>, capturing shocks and energy transfer into the ambient medium;</li>
    <li><strong>Particle transport in the Galactic environment</strong>, tracking propagation and cooling once particles leave the jet;</li>
    <li><strong>Detector-space predictions</strong>, folding outputs through <strong>CTA</strong> and <strong>KM3NeT</strong> responses to forecast detectable signatures.</li>
  </ul>
  <p>This program aims to compare <strong>microquasars and SMBHs</strong> to clarify jet acceleration and jet-environment coupling under different scales and conditions.</p>
</section>

<section class="site-section">
  <h2>Visual Context</h2>
  <div class="site-figure-grid">
    <figure>
      <img src="/images/V4641.jpg" alt="V4641 Sgr">
      <figcaption><em>V4641 Sgr, a microquasar used to probe jet acceleration and jet-medium interaction. Credit: StarDate.</em></figcaption>
    </figure>
    <figure>
      <img src="/images/jet.jpg" alt="Astrophysical jet interacting with surrounding medium">
      <figcaption><em>Jet-medium interaction: where acceleration, shocks, and transport imprint observable multi-messenger signatures.</em></figcaption>
    </figure>
  </div>
</section>

<section class="site-section site-callout">
  <h2>Blog and Group Writing</h2>
  <p>Short research notes, group-style posts, and selected updates can live on the blog without crowding the research overview.</p>
  {% if site.posts.size > 0 %}
  <ul class="site-post-list">
    {% for post in site.posts limit:3 %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span>{{ post.date | date: "%d %b %Y" }}</span>
    </li>
    {% endfor %}
  </ul>
  {% else %}
  <p class="site-muted">No blog posts are published yet.</p>
  {% endif %}
</section>
