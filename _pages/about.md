---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am **Tony** (Haoze) Guo, currently pursuing my Bachelor of Science in **Computer Engineering** and **Computer Science** with **honor** at the **[University of Wisconsin–Madison](https://www.cs.wisc.edu/)**, expecting to graduate in May 2027.

My primary research interests include **Human-Computer Interaction (HCI)**, **Natural Language Processing (NLP)**, **Social Computing**, and **AI-powered interactive systems**. I'm particularly passionate about creating intuitive, scalable, and user-centered interactive technologies.

Currently, I am leading frontend optimization efforts for **VirT-Lab**, an AI-powered multi-agent simulation platform, supervised by **[Prof. Diego Gómez-Zará](https://engineering.nd.edu/faculty/diego-gomez-zara/)**. My role involves enhancing real-time interactions and visualization capabilities to support effective human-AI collaboration.

Feel free to explore my website for more details on my research projects, publications, and technical background!

---

NEWS
======
- *2025-07-11*
> We successfully submitted our paper to **UIST Demo '25** 🎉
- *2025-06-01*
> Join the RINGZ-Lab as an iSURE student advised by **Prof. Diego Gómez-Zará** 🎉
- *2023-09-06*
> Begun my undergraduate study at **University of Wisconsin - Madison** 🎉

---

Courses & Skills
======

**Core Coursework (Completed / In Progress)**

- *CS / CE Foundations:* Data Structure and Analysis; Algorithms; Systems Programming; Software Engineering; Software Design; Computer Organization & Architecture; Artificial Intelligence; Database Management; Computer Vision (INP); Robotic System (INP); Mobile App Dev (INP)

- *Math & Theory:* Probability & Statistics; Discrete Math; Linear Algebra; Multivariable Calc

**Programming Languages (Proficient):** Python · JavaScript/TypeScript · Java · C/C++ · SQL · Go · MATLAB · R · C# 

**Frameworks / Libraries:** React · Node.js / Express · PyTorch · Vue.js

**Developer & Cloud Tools:** Git · Linux · AWS(Lambda) · Google Cloud Platform · Docker · pyCharm · VS Code · Unity Hub

---

## Selected Publications
{% assign you = "Haoze Guo" %}
{% capture you_tag %}<mark>{{ you }}</mark>{% endcapture %}
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
