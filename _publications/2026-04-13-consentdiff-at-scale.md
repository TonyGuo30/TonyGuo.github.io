---
layout: single
title: "ConsentDiff at Scale: Longitudinal Audits of Web Privacy Policy Changes and UI Frictions"
authors:
  - Haoze Guo
date: 2026-04-13
collection: publications
category: conferences
permalink: /publication/consentdiff-at-scale

# card fields
venue: "ACM CHI Conference on Human Factors in Computing Systems Extended Abstracts"
abbr: "CHI EA '26"
paperurl: "https://dl.acm.org/doi/pdf/10.1145/3772363.3798570"
abstract: >
  Web privacy is experienced via two public artifacts: site utterances in policy texts,
  and the actions users are required to take during consent interfaces. In the extensive
  cross-section audits we've studied, there is a lack of longitudinal data detailing
  how these artifacts are changing together, and if interfaces are actually doing what
  they promise in policy. ConsentDiff provides that longitudinal view. We build a
  reproducible pipeline that snapshots sites every month, semantically aligns policy
  clauses to track clause-level churn, and classifies consent-UI patterns by pulling
  together DOM signals with cues provided by screenshots. We introduce a novel weighted
  claim-UI alignment score, connecting common policy claims to observable predicates,
  and enabling comparisons over time, regions, and verticals. Our measurements suggest
  continued policy churn, systematic changes to eliminate a higher-friction banner
  design, and significantly higher alignment where rejecting is visible and lower
  friction.
bibtex: |
  @inproceedings{10.1145/3772363.3798570,
  author = {Guo, Haoze},
  title = {ConsentDiff at Scale: Longitudinal Audits of Web Privacy Policy Changes and UI Frictions},
  year = {2026},
  isbn = {9798400722813},
  publisher = {Association for Computing Machinery},
  address = {New York, NY, USA},
  url = {https://doi.org/10.1145/3772363.3798570},
  doi = {10.1145/3772363.3798570},
  abstract = {Web privacy is experienced via two public artifacts: site utterances in policy texts, and the actions users are required to take during consent interfaces. In the extensive cross-section audits we've studied, there is a lack of longitudinal data detailing how these artifacts are changing together, and if interfaces are actually doing what they promise in policy. ConsentDiff provides that longitudinal view. We build a reproducible pipeline that snapshots sites every month, semantically aligns policy clauses to track clause-level churn, and classifies consent-UI patterns by pulling together DOM signals with cues provided by screenshots. We operationalize claim-UI alignment by mapping policy claims to observable UI predicates, connecting common policy claims to observable predicates, and enabling comparisons over time, regions, and verticals. Our measurements suggest continued policy churn, systematic changes to eliminate a higher-friction banner design, and significantly higher alignment where rejecting is visible and lower friction.},
  booktitle = {Proceedings of the Extended Abstracts of the 2026 CHI Conference on Human Factors in Computing Systems},
  articleno = {185},
  numpages = {5},
  keywords = {privacy policies, consent management platforms (CMPs), cookie banners, dark patterns},
  location = {},
  series = {CHI EA '26}
  }
---
