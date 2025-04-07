---

---
# USS Hanesawa Computer Library

{% capture bluethrobber %}
  {% include throbber.html %}
  {: .blued.widen}
{% endcapture %}

<div class="flexbox">
  <div class="col"> 
    {{ bluethrobber | markdownify }}
  </div>
  <div class="col">
    <h2 class="font-almond-creme">Access Granted</h2>
    <div class="lcars-text-bar">
      <span>Recent Missions</span>
    </div>
    <div class="buttons jc-space-around">
      {% for post in site.categories['mission'] limit:4 %}   
        <a class="button-{% cycle 'bluey', 'peach', 'violet-creme', 'lima-bean' %} {% if forloop.first %}blink{% endif %}" href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
      {% endfor %}
    </div>
  </div>
</div>