---
title: "Research"
permalink: /research/
author_profile: true
---

## Working papers

{% for pub in site.data.JMP %}
  **[{{pub.title}}]({{pub.link}}){:target="_blank"}** \
  (with {% for author in pub.coauthors %} {% if author.link %}[{{ author.name }}]({{ author.link }}){:target="_blank"}{% else %}{{ author.name }}{% endif %}{% unless forloop.last %}, {% endunless %}{% endfor %}) \
  *{{ pub.publication }}*
  <!-- This applies apply the no-margins class to prev paragraph to remove margins -->
  {: class="no-margins"}
  <details>
      <summary>Abstract (click to expand)</summary>
      {{ pub.abstract }}
  </details>

  <!-- This creates line break to space out items; need the no-margins class also since this gets automatically wrapped with a <p> which by default has extra margins -->
  <br/>
  {: class="no-margins"}
{% endfor %}

{% for pub in site.data.WP %}
  **[{{pub.title}}]({{pub.link}}){:target="_blank"}** \
  (with {% for author in pub.coauthors %} {% if author.link %}[{{ author.name }}]({{ author.link }}){:target="_blank"}{% else %}{{ author.name }}{% endif %}{% unless forloop.last %}, {% endunless %}{% endfor %}) \
  *{{ pub.publication }}*
  <!-- This applies apply the no-margins class to prev paragraph to remove margins -->
  {: class="no-margins"}
  <details>
      <summary>Abstract (click to expand)</summary>
      {{ pub.abstract }}
  </details>

  <!-- This creates line break to space out items; need the no-margins class also since this gets automatically wrapped with a <p> which by default has extra margins -->
  <br/>
  {: class="no-margins"}
{% endfor %}
