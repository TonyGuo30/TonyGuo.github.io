---
layout: single
title: "Hidden-in-Plain-Text: A Benchmark for Social-Web Indirect Prompt Injection in RAG"
authors:
  - Haoze Guo
  - Ziqi Wei
date: 2026-01-16
collection: publications
category: conferences
permalink: /publication/Hidden-in-Plain-Text

# — card fields — #
venue: "The Web Conference (WWW)"
abbr: "WWW '26"
preview: /images/Hidden.png
paperurl: "https://arxiv.org/pdf/2601.10923"
figlink: "https://arxiv.org/abs/2601.10923"
abstract: >
  Retrieval-augmented generation (RAG) systems put more and more emphasis on grounding their
  responses in user-generated content found on the Web, amplifying both their usefulness 
  and their attack surface…
altmetric: 248277
---

<!-- Minimal inline style so the hero image pops even if custom.scss isn't loaded -->
<style>
  .pub-hero{margin:1rem 0 1.25rem}
  .pub-thumb-link{display:inline-block;line-height:0;border-radius:12px;text-decoration:none}
  .pub-thumb-link img{display:block;border-radius:12px;box-shadow:0 2px 10px rgba(0,0,0,.08);transition:transform .18s ease,box-shadow .18s ease}
  .pub-thumb-link:hover img,.pub-thumb-link:focus img{transform:translateY(-2px) scale(1.04);box-shadow:0 12px 30px rgba(0,0,0,.2)}
  .pub-thumb-link:focus{outline:2px solid currentColor;outline-offset:3px}
</style>

<!-- Big hero image on the individual publication page -->
<div class="pub-hero">
  <a class="pub-thumb-link" href="{{ page.figlink | default: page.paperurl }}" target="_blank" rel="noopener">
    <img src="{{ page.preview | relative_url }}" alt="privacy-recall" loading="lazy">
  </a>
</div>
