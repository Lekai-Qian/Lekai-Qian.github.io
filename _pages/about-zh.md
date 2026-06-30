---
permalink: /zh/
author_profile: true
title: ""
lang: zh
---

<span style="color: #003366; font-weight: bold; font-size: 0.7em;">关于我</span>
======
我是华南理工大学未来技术学院人工智能专业的大三本科生,师从 [Prof. Qi Liu (刘琦教授)](https://drliuqi.github.io/)。同时,我也与 [Music X Lab](https://www.musicxlab.com/#/) 保持紧密合作,由 [Prof. Gus Xia](https://www.musicxlab.com/members/gus/) 与 [Dr. Ziyu Wang](https://zzwaang.github.io/) 联合指导。

<span style="color: #003366; font-weight: bold; font-size: 0.7em;">研究兴趣</span>
======
我的研究方向位于**表征学习**与**生成式模型**的交叉点。从宽泛的层面看,我致力于学习高质量的语义表征,以服务于扩散模型、自回归模型等生成式方法,提升其在**多模态数据**上的建模与生成能力。

具体而言,我以**符号音乐**作为这一研究主线的切入点,研究表征与 tokenization 的设计如何决定生成模型能够学习、创作和控制的内容。我尤其关注超越传统事件序列(event-sequence)的表征形式,探索能够更忠实地反映音乐时间、结构与多声部特性的方法。

<span style="color: #003366; font-weight: bold; font-size: 0.7em;">动态</span>
======
- **2026 年 5 月**:我们的论文 *BEAT* 被 ICML 2026 接收。
- **2026 年 1 月**:我们的论文 *Pianoroll-Event* 被 ICASSP 2026 接收。

<div id="publications"></div>
<span style="color: #003366; font-weight: bold; font-size: 0.7em;">发表论文</span>
======
{% if site.author.googlescholar %}你也可以在 <a href="{{site.author.googlescholar}}">我的 Google Scholar 主页</a> 找到我的论文。{% endif %}
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
