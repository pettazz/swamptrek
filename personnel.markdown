---
title: "Personnel"
---

## USS Hanesawa

{% assign players = site.personnel | where: "crew", true | where: "pc", true %}

<div class="lcars-text-bar">
  <span>Senior Staff</span>
</div>

<ul class="lcars-list">
{% for person in players %}
  {% assign roles = person.roles | map: "name" | join: "/" %}
  <li>{{ roles }} <a href="{{person.url}}">{{ person.rank }} {{ person.full_name }}</a></li>
{% endfor %}
</ul>

{% assign crew = site.personnel | where: "crew", true | where: "pc", false %}

{% unless crew == empty %}
  <div class="lcars-text-bar">
    <span>Crew</span>
  </div>

  <ul class="lcars-list">
  {% for person in crew %}
    {% assign roles = person.roles | map: "name" | join: "/" %}
    <li>{{ roles }} <a href="{{person.url}}">{{ person.rank }} {{ person.full_name }}</a></li>
  {% endfor %}
  </ul>
{% endunless %}

## Other Characters

{% assign factions = site.personnel | map: "alignment" | uniq %}

{% for faction in factions %}

  <div class="lcars-text-bar">
    <span>{{ faction }}</span>
  </div>

  {% assign faction_people = site.personnel | where: "alignment", faction | where: "crew", false %}

  <ul class="lcars-list">
  {% for person in faction_people %}
    <li><a href="{{ person.url }}">{{ person.rank }} {{ person.full_name }}</a></li>
  {% endfor %}
  </ul>


{% endfor %}
