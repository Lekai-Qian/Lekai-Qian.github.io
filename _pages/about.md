---
permalink: /
author_profile: true
title: ""
redirect_from:
  - /about/
  - /about.html
---

<span style="color: #003366; font-weight: bold; font-size: 0.7em;">About Me</span>
======
I am a third-year undergraduate at the School of Future Technology, South China University of Technology, majoring in Artificial Intelligence and advised by [Prof. Qi Liu](https://drliuqi.github.io/). I also work closely with [Music X Lab](https://www.musicxlab.com/#/), where I am co-supervised by [Prof. Gus Xia](https://www.musicxlab.com/members/gus/) and [Dr. Ziyu Wang](https://zzwaang.github.io/).

<span style="color: #003366; font-weight: bold; font-size: 0.7em;">Research Interests</span>
======
My research lies at the intersection of **representation learning** and **generative modeling**. Broadly, I aim to learn high-quality semantic representations that empower generative methods — such as diffusion and autoregressive models — to model and generate **multimodal data** more effectively.

Concretely, I ground this agenda in **symbolic music**, where I study how the choice of representation and tokenization shapes what generative models can learn, compose, and control. I am particularly interested in moving beyond event-sequence formulations toward representations that more faithfully capture musical time, structure, and polyphony.

<span style="color: #003366; font-weight: bold; font-size: 0.7em;">News</span>
======
- **May 2026**: Our paper *BEAT* has been accepted by ICML 2026.
- **Jan 2026**: Our paper *Pianoroll-Event* has been accepted by ICASSP 2026.

<div id="publications"></div>
<span style="color: #003366; font-weight: bold; font-size: 0.7em;">Publications</span>
======
{% if site.author.googlescholar %}You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.{% endif %}
<ul style="list-style: none; padding-left: 0;">
{% assign sorted_pubs = site.publications | sort: 'date' | reverse %}
{% for post in sorted_pubs %}
  <li style="margin-bottom: 1.5em; line-height: 1.6;">
    {{ post.authors | replace: 'Lekai Qian', '<b>Lekai Qian</b>' }}.
    {{ post.title | remove: '"' }}.
    <i>{{ post.venue }}</i>, {{ post.date | date: "%Y" }}.
    {% if post.paperurl %} [<a href="{{ post.paperurl }}">paper</a>]{% endif %}
    {% if post.demourl %} [<a href="{{ post.demourl }}">demo</a>]{% endif %}
    {% if post.codeurl %} [<a href="{{ post.codeurl }}">code</a>]{% endif %}
    {% if post.slidesurl %} [<a href="{{ post.slidesurl }}">slides</a>]{% endif %}
    {% if post.bibtexurl %} [<a href="{{ post.bibtexurl }}">bibtex</a>]{% endif %}
  </li>
{% endfor %}
</ul>
