---
layout: single
title: "VirT-Lab: An AI-Powered System for Flexible, Customizable, and Large-Scale Team Simulations"
authors:
  - Mohammed Almutairi
  - Charles Chiang
  - Haoze Guo
  - Matthew Belcher
  - Nandini Banerjee
  - Maria Milkowski
  - Svitlana Volkova
  - Daniel Nguyen
  - Tim Weninger
  - Michael Yankoski
  - Trenton W. Ford
  - Diego Gomez-Zara
date: 2025-07-18
collection: publications
category: conferences
permalink: /publication/virt-lab-2025-uist-demo

# — card fields — #
venue: "ACM Symposium on User Interface Software and Technology (UIST) 2025 Demo"
abbr: "UIST '25"
preview: /images/virtlab-thumb.gif
paperurl: "https://arxiv.org/pdf/2508.04634v1"
abstract: >
  We introduce **VirT-Lab**, a user-friendly, customizable, multi-agent
  simulation system that leverages LLM agents in spatial and temporal
  environments …
altmetric: 248277
selected: true
---

<!-- Inline styles so the hover/click effect works even without _custom.scss -->
<style>
  .pub-hero { margin: 1rem 0 1.25rem; }
  .pub-hero a {
    display: inline-block;
    position: relative;
    text-decoration: none;
    line-height: 0; /* trims stray whitespace; safe if image loads */
    border-radius: 14px;
    cursor: pointer;
  }
  /* Works for <img>, <svg>, <figure>, or an element with .sig */
  .pub-hero a > img,
  .pub-hero a > svg,
  .pub-hero a > figure,
  .pub-hero a > .sig {
    display: block;
    max-width: min(100%, 560px);
    height: auto;
    border-radius: 12px;
    box-shadow: 0 2px 10px rgba(0,0,0,.08);
    transition: transform .18s ease, box-shadow .18s ease;
    will-change: transform;
  }
  .pub-hero a:hover > img,
  .pub-hero a:focus > img,
  .pub-hero a:focus-visible > img,
  .pub-hero a:hover > svg,
  .pub-hero a:focus > svg,
  .pub-hero a:focus-visible > svg,
  .pub-hero a:hover > figure,
  .pub-hero a:focus > figure,
  .pub-hero a:focus-visible > figure,
  .pub-hero a:hover > .sig,
  .pub-hero a:focus > .sig,
  .pub-hero a:focus-visible > .sig {
    transform: translateY(-2px) scale(1.04);
    box-shadow: 0 12px 30px rgba(0,0,0,.2);
  }
  .pub-hero a:focus,
  .pub-hero a:focus-visible {
    outline: 2px solid currentColor;
    outline-offset: 4px;
  }
  .pub-cta {
    display: inline-block;
    margin-top: .6rem;
    font-weight: 600;
    text-decoration: none;
    border-bottom: 1px solid currentColor;
  }
  @media (prefers-reduced-motion: reduce) {
    .pub-hero a > img,
    .pub-hero a > svg,
    .pub-hero a > figure,
    .pub-hero a > .sig { transition: none; }
  }
</style>

<div class="pub-hero">
  <a href="{{ page.paperurl }}" target="_blank" rel="noopener">
    <!-- Using relative_url so it works on GitHub Pages with baseurl -->
    <img src="{{ page.preview | relative_url }}" alt="VirT-Lab demo thumbnail" loading="lazy">
  </a>
</div>

<p><a class="pub-cta" href="{{ page.paperurl }}" target="_blank" rel="noopener">Open paper →</a></p>
