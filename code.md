---
title: code
---
<div class="page-content-container">
  <header>
    <p>collection of my open-source contributions and projects.</p>
    <a href="/closed-source"><p style="padding: 0.5em 0;">click here for closed source mentions.</p></a>
  </header>

  <hr class="page-content-divider">

  <section class="page-content-collection-container">
    {% assign open_source_by_year = site.open_source | sort: "year" | reverse %}
    {% for project in open_source_by_year %}
    <a class="page-content-collection-item code-project-url" href="{{ project.url }}">
      <h2><span class="monokai-symbol">{{ project.kind }}</span> <span class="monokai-constant">{{ project.title }}</span></h2>
      <p class="monokai-string">"{{ project.description }}"</p>
      (<span class="monokai-number">{{ project.year }}</span>)
    </a>
    {% endfor %}
  </section>
</div>
