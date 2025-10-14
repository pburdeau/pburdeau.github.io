---
layout: splash
title: "Philippine Burdeau"
permalink: /
header:
  overlay_color: "#0a2540"
  overlay_filter: 0.45
  overlay_image: /assets/img/hero.jpg
  actions:
    - label: "Download CV"
      url: /assets/cv/Philippine_Burdeau_CV.pdf
excerpt: >
  I build statistical & geospatial methods for **methane emissions** and **produced gas composition**—combining
  measurements and inventories to improve basin-scale estimates. Now in Boston and open to R&D/TPM roles in climatetech.
intro: 
  - excerpt: >
      <span style="font-size:1.05rem">
      Focus areas: **intermittency/HMMs**, **kriging + non-linear models**, and **reproducible pipelines**.
      Current basins: Permian, Anadarko, Haynesville, Appalachian.
      </span>
feature_row:
  - image_path: /assets/img/thumb_research.jpg
    alt: "Research"
    title: "Research"
    excerpt: "Methods + applications for emissions & composition."
    url: "/research/"
    btn_label: "See projects"
    btn_class: "btn--primary"
  - image_path: /assets/img/thumb_pubs.jpg
    alt: "Publications"
    title: "Publications"
    excerpt: "Papers, preprints, and datasets."
    url: "/publications/"
    btn_label: "Read more"
  - image_path: /assets/img/thumb_news.jpg
    alt: "News"
    title: "News"
    excerpt: "Talks, travels, releases."
    url: "/news/"
    btn_label: "Latest"
---

{% include feature_row id="feature_row" %}

<div class="grid" style="margin-top:1.2rem">
  <div class="card">
    <h3>Highlights</h3>
    <ul>
      <li><b>Nature Communications</b> — produced gas composition paper (in principle, 2025).</li>
      <li>DOE/Stanford/LBNL collaborations on basin-level inventories.</li>
      <li>Open, reproducible code & maps (Python + Deck.gl).</li>
    </ul>
  </div>

  <div class="card">
    <h3>What I’m looking for</h3>
    <p>Collaborations and roles at the intersection of emissions, sensing, and geospatial modeling.</p>
    <p><a href="/contact/">Get in touch →</a></p>
  </div>

  <div class="card">
    <h3>Recent news</h3>
    <ul>
      {%- assign latest = site.news | sort: 'date' | reverse | slice: 0,3 -%}
      {%- for item in latest -%}
      <li><a href="{{ item.url }}">{{ item.title }}</a> <small>({{ item.date | date: "%b %Y" }})</small></li>
      {%- endfor -%}
    </ul>
  </div>
</div>