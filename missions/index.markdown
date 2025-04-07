---
title: "Mission History"
---

{% for post in site.categories['mission'] %}
  <div class="lcars-text-bar">
    <span>{{ post.title }}</span>
  </div>
  <strong>EARTH DATE:</strong> {{ post.date | date: "%B %d, %Y" }} <br />
  <strong>STARDATE:</strong> {{ post.stardate }}
  <div class="buttons">
    <a class="button-peach" href="{{ site.url }}{{ post.url }}">View log</a>
  </div>
{% endfor %}

