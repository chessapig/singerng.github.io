---
title: Talks
permalink: /talks
layout: default
---

# Talks
<br/>

{% for talk in site.data.talks %}
  <div class="card mb-3">
    <div class="card-body">
      <a href="/talks/{{ talk.slides }}" target="_blank" class="text-dark"><h5 class="card-title">{{ talk.title }}</h5></a>
      <h6 class="card-subtitle mb-2 text-muted"><strong> {{ talk.authors }}</strong> &mdash; {{ talk.date |  date: "%A, %B %d, %Y" }} &mdash; <em>{{ talk.venue }}</em></h6>
    </div>
  </div>
{% endfor %}
