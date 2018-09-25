---
layout: default
title: SeniorSem
---

{% for sem in site.seniorSem %}


<a href="{{ sem.url | prepend: site.baseurl }}">
        <h2>{{ sem.title }}</h2>
</a>

<p class="post-excerpt">{{ sem.description | truncate: 160 }}</p>

{% endfor %}      
