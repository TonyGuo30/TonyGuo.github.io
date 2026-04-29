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

> 📢 **I am actively looking for research opportunities in HCI related field! And also planning to PHD or Master degree!**
{: .fancy}

---

## News

<section class="news-panel" aria-label="Recent news">
  <div class="news-panel__header">
    <div>
      <span class="news-panel__eyebrow">Latest Updates</span>
      <h3>Recent Highlights</h3>
    </div>
    <span class="news-panel__count">5 updates</span>
  </div>

  <div class="news-feed">
    <article class="news-card news-card--featured">
      <time datetime="2026-01-04">Jan 04, 2026</time>
      <p>My paper was accepted by <strong>WWW '26</strong>.</p>
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
{% assign you = "Haoze Guo" %}
{% capture you_tag %}<strong>{{ you }}</strong>{% endcapture %}
{% assign sel = site.publications | where: "selected", true | sort: "date" | reverse %}

<div class="pub-list">
{% for p in sel %}
  {%- assign authors = p.authors | split: "," -%}
  {%- assign last_author = authors | last -%}
  {%- capture trimmed_authors -%}
    {%- for a in authors -%}
      {%- assign nm = a | strip -%}
      {%- if nm contains you -%}
        {{ nm }}{%- unless last_author contains you -%}, …]{%- endunless -%}
        {%- break -%}
      {%- else -%}
        {{ nm }},
      {%- endif -%}
    {%- endfor -%}
  {%- endcapture -%}

  <div class="pub-item">
    {% if p.preview %}
      <div class="pub-thumb">
        <img src="{{ p.preview | relative_url }}" alt="preview of {{ p.title }}">
      </div>
    {% endif %}

    <div class="pub-body">
      {% if p.abbr %}<span class="pub-badge">{{ p.abbr }}</span>{% endif %}
      <span class="pub-authors">
        {{ trimmed_authors | strip | replace: you, you_tag }}.
      </span>
      <span class="pub-year"> {{ p.date | date: "%Y" }}.</span>
      <span class="pub-title"><i>{{ p.title }}</i>.</span>
      {% if p.venue %}<span class="pub-venue"> {{ p.venue }}.</span>{% endif %}

      <div class="pub-links">
        {% if p.paperurl %}<a href="{{ p.paperurl | relative_url }}">PDF</a>{% endif %}
      </div>
    </div>
  </div>
  <hr>
{% endfor %}
</div>
