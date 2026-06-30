---
title: "Pianoroll-Event: A Novel Score Representation for Symbolic Music"
collection: publications
category: conferences
permalink: /publication/2026-pianoroll-event
date: 2026-01-26
venue: 'ICASSP'
header:
  teaser: paper_icassp.png
authors: 'Lekai Qian, Haoyu Gu, Dehan Li, Boyu Cao, Qi Liu'
paperurl: 'https://arxiv.org/abs/2601.19951'
demourl: 'https://akualubi.github.io/PIANOROLL-EVENT/'
---

<div align="center">
  <img src="{{ site.baseurl }}/images/paper_icassp.png" alt="Pianoroll-Event Framework" style="width: 100%; max-width: 900px;">
  <p><em>Overview of the Pianoroll-Event encoding pipeline: from pianoroll to compressed event sequence.</em></p>
</div>

## Abstract

We introduce an encoding scheme that merges pianoroll representations with event-based descriptions. Our approach defines four event types:

| Event Type | Description |
|------------|-------------|
| **Frame Events** | Capture temporal structure of musical segments |
| **Gap Events** | Handle silence and rests between notes |
| **Pattern Events** | Encode repetitive musical patterns efficiently |
| **Structure Events** | Represent high-level musical form |

This scheme achieves **1.36x to 7.16x encoding efficiency** compared to comparable discrete sequence approaches. Testing across multiple autoregressive models demonstrates consistent performance gains in both objective metrics and human evaluation.

## Links

- [Paper (arXiv)](https://arxiv.org/abs/2601.19951)
- [PDF](https://arxiv.org/pdf/2601.19951)
