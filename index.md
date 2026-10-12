---
title: About
heading: About Me
permalink: /
---

My background is in Industrial Engineering at [Sharif University of Technology](https://en.sharif.edu/) (B.Sc., 2021–2026), where I ranked first in my class, with a minor in Economics.

I am interested in how mathematical models and data can support better decisions in real systems. My work spans **operations research, stochastic modeling, and applied economics**: from optimization models for production scheduling and taxi-fleet repositioning, to a discrete-event simulation of patient flow in a hospital, to an econometric study of income inequality and crime across U.S. states.

## Research Interests

- Operations research and mathematical optimization
- Stochastic modeling and queueing systems
- Simulation of service and healthcare systems
- Econometrics and applied economics
- Data-driven decision-making

## Working Papers

{% include publications.html %}

## Education

<div class="entries">
{%- for e in site.data.education %}
  <div class="entry">
    <div class="entry-head">
      <p class="entry-title">{{ e.degree }}</p>
      <p class="entry-dates">{{ e.dates }}</p>
    </div>
    <p class="entry-sub">{% if e.url %}<a href="{{ e.url }}">{{ e.institution }}</a>{% else %}{{ e.institution }}{% endif %}{% if e.location %}, {{ e.location }}{% endif %}</p>
    {%- if e.details %}<p class="entry-body">{{ e.details | join: " &middot; " }}</p>{% endif %}
  </div>
{%- endfor %}
</div>
