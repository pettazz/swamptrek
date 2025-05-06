---
title: "Mission History"
---

{% for post in site.categories['mission'] %}
  <div class="lcars-text-bar">
    <span>{{ post.title }}</span>
  </div>

  <div class="flexbox">
    <div class="col">
      <strong>EARTH DATE:</strong> {{ post.date | date: "%B %d, %Y" }} <br />
      <strong>STARDATE:</strong> {{ post.stardate }}
    </div>
    <div class="col">
      <div class="buttons">
        <a class="button-peach" href="{{ site.url }}{{ post.url }}">View log</a>
      </div>
    </div>
  </div>
{% endfor %}

