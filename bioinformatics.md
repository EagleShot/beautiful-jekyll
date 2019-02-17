---
layout: default
title: Bioinformatics
---

{% for bio in site.bioinformatics %}


<a href="{{ bio.url | prepend: site.baseurl }}">
        <h2>{{ bio.title }}</h2>
</a>

<p class="post-excerpt">{{ bio.description | truncate: 160 }}</p>

{% endfor %}
