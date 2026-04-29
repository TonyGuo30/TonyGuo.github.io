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
bibtex: |
  @inproceedings{10.1145/3774904.3792853,
  author = {Guo, Haoze and Wei, Ziqi},
  title = {Hidden-in-Plain-Text: A Benchmark for Social-Web Indirect Prompt Injection in RAG},
  year = {2026},
  isbn = {9798400723070},
  publisher = {Association for Computing Machinery},
  address = {New York, NY, USA},
  url = {https://doi.org/10.1145/3774904.3792853},
  doi = {10.1145/3774904.3792853},
  abstract = {Retrieval-augmented generation (RAG) systems increasingly ground responses in user-generated Web content, expanding both usefulness and attack surface. Two web-native threats are especially concerning: indirect prompt injection and retrieval poisoning, where malicious instructions or biased content survive ingestion and influence retrieval or generation. We introduce OpenRAG-Soc, a compact, reproducible benchmark and harness for evaluating web-facing RAG pipelines under these threats as a discrete data package. The suite pairs a social corpus with interchangeable sparse and dense retrievers and deployable mitigations, including HTML/Markdown sanitization, Unicode normalization, and attribution-gated answering. OpenRAG-Soc standardizes end-to-end evaluation from ingestion to generation and reports attack success at answer time, rank shifts in both sparse and dense retrievers, as well as utility and latency. It targets practitioners who need fast, realistic tests to measure risk and harden RAG deployments.},
  booktitle = {Proceedings of the ACM Web Conference 2026},
  pages = {8337–8340},
  numpages = {4},
  keywords = {retrieval-augmented generation, prompt injection, web security, social web, poisoning attacks, llm safety},
  location = {United Arab Emirates},
  series = {WWW '26}
  }
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
