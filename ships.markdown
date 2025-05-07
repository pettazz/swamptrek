---
title: "Starship Registry"
---

{% assign fleets = site.ships | map: "alignment" | uniq %}

{% for fleet in fleets %}

  <div class="lcars-text-bar">
    <span>{{ fleet }}</span>
  </div>

  {% assign fleet_ships = site.ships | where: "alignment", fleet %}

  <ul class="lcars-list">
  {% for ship in fleet_ships %}
    <li><a href="{{ ship.url }}">{{ ship.ship_name }} - {{ ship.registry }}</a></li>
  {% endfor %}
  </ul>

{% endfor %}