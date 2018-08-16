---
layout: landing
title: top
---
<div class="landing-msg">
  <h1>trevor malard</h1>
  <p>digital creative</p>
  {% assign landing_links = site.links %}

  {% for link in landing_links %}
    <br><a href="/{{ link }}"><div class="landing-link">{{ link }}</div></a>
  {% endfor %}
</div>
