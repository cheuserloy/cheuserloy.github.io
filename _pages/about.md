---
permalink: /
title: "The Immunoengineering Lab"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
## Research
<p align="justify">Our research focuses on boosting the functional persistence of T cells to develop innovative adoptive cell therapies.
By diving deep into the biology of functional, exhausted, and engineered CD8<sup>+</sup> T cells, we uncover critical metabolic, genetic, and epigenetic switches that control their fate. Harnessing these master regulators, we re-engineer T cells and explore how they adapt and respond to different signals and environments, paving the way for more powerful and durable immunotherapies.</p>
---

## Latest news

{% assign latest_news = site.news | sort: "date" | reverse | slice: 0, 3 %}

{% for item in latest_news %}

### [{{ item.title }}]({{ item.url | relative_url }})

<small>{{ item.date | date: "%d %B %Y" }}</small>

{{ item.excerpt | strip_html | truncate: 220 }}

{% endfor %}

[All news &rarr;]({{ '/news/' | relative_url }})
