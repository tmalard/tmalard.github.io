---
title: top
---
<div id="landing-page">
  <div class="landing-msg">
    <h1>trevor malard</h1>
    <div class="tagline">
      <h2>digital creative</h2>
      <p>tokyo/los angeles</p>
    </div>
    {% assign landing_links = site.links %}

    {% for link in landing_links %}
      <a href="/{{ link }}">
        <div class="landing-link">{{ link }}</div>
      </a>
    {% endfor %}
  </div>
</div>
