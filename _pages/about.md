---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am **Tony** (Haoze) Guo, currently pursuing my Bachelor of Science in **Computer Engineering** and **Computer Science** with **honor** at the **[University of Wisconsin–Madison](https://www.cs.wisc.edu/)**, expecting to graduate in May 2027.

My primary research interests include **Human-Computer Interaction (HCI)**, *Natural Language Processing (NLP)*, *Computational Social Science*, and **AI-powered interactive systems**. I'm particularly passionate about creating intuitive, scalable, and user-centered interactive technologies.

Currently, I am leading frontend development and backend optimization efforts for **VC-LLM**, an tree structured, LLM chat platform, supervised by **[Prof. Bilge Mutlu](https://bmutlu.github.io/)**. My role involves building the interface for the system, and optimizing the backend fatures for the system.

Feel free to explore my website for more details on my research projects, publications, and technical background!

<div class="opportunity-callout">
  <span class="opportunity-callout__label">📢 Open to opportunities</span>
  <p>I am currently seeking research opportunities in HCI and AI-powered interactive systems, especially roles that could support my path toward graduate study.</p>
</div>

---

## News

<section class="news-panel" aria-label="Recent news">
  <div class="news-feed">
    <article class="news-card news-card--featured">
      <time datetime="2026-04-18">Apr 18, 2026</time>
      <p>My paper <strong>Behind the Feed</strong> was accepted to <strong>ESCSW Poster '26</strong>.</p>
    </article>

    <article class="news-card">
      <time datetime="2026-04-13">Apr 13, 2026</time>
      <p>My paper <strong>ConsentDiff at Scale</strong> was accepted to <strong>CHI EA '26</strong>.</p>
    </article>

    <article class="news-card">
      <time datetime="2026-01-04">Jan 04, 2026</time>
      <p>My paper <strong>Hidden-in-Plain-Text</strong> was accepted by <strong>WWW '26</strong>.</p>
    </article>

    <article class="news-card">
      <time datetime="2025-09-18">Sep 18, 2025</time>
      <p>I will join the <strong>IUI '26 PC</strong> as a reviewer.</p>
    </article>

    <article class="news-card">
      <time datetime="2025-08-02">Aug 02, 2025</time>
      <p>Our paper was conditionally accepted by <strong>UIST Demo '25</strong>.</p>
    </article>

    <article class="news-card">
      <time datetime="2025-06-01">Jun 01, 2025</time>
      <p>Joined the RINGZ-Lab as an iSURE student advised by <strong>Prof. Diego Gómez-Zará</strong>.</p>
    </article>

    <article class="news-card">
      <time datetime="2023-09-06">Sep 06, 2023</time>
      <p>Began my undergraduate study at <strong>University of Wisconsin - Madison</strong>.</p>
    </article>
  </div>
</section>

---

## Selected Publications
{% assign sel = site.publications | where: "selected", true | sort: "date" | reverse %}

<div class="publication-list publication-list--selected">
{% for p in sel %}
  {% include pub_card.html page=p %}
{% endfor %}
</div>
