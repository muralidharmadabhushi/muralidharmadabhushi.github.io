---
layout: default
title: Publications
nav_id: publications
permalink: /publications.html
---

### Publications

<div class="pub-tabs" aria-label="Publication views">
  <input type="radio" id="pub-tab-featured" name="pub-tabs" checked />
  <label for="pub-tab-featured">Featured</label>

  <input type="radio" id="pub-tab-year" name="pub-tabs" />
  <label for="pub-tab-year">By year</label>

  <section class="pub-panel pub-panel-featured" aria-label="Featured publications">
    {% assign featured_publications = site.publications | where: "featured", true %}
    {% for pub in featured_publications %}
      <article class="featured-publication-card">
        {% if pub.thumbnail and pub.thumbnail != "" %}
          <img src="{{ pub.thumbnail | relative_url }}" alt="Thumbnail for {{ pub.title }}" />
        {% endif %}
        <div class="featured-publication-body">
          <div class="publication-title">{{ pub.title }}</div>
          <div class="publication-meta">{{ pub.venue }} · {{ pub.year }}</div>
          {% if pub.link and pub.link != "" and pub.link != "#" %}
            <div class="publication-links"><a href="{{ pub.link }}">Link</a></div>
          {% endif %}
          {% if pub.tldr and pub.tldr != "" %}
            <p><strong>TL;DR:</strong> {{ pub.tldr }}</p>
          {% endif %}
        </div>
      </article>
    {% endfor %}
  </section>

  <section class="pub-panel pub-panel-year" aria-label="Publications by year">
    {% assign publications_by_year = site.publications | group_by: "year" | sort: "name" | reverse %}
    {% for year_group in publications_by_year %}
    <h3>{{ year_group.name }}</h3>
    <ul>
      {% for pub in year_group.items %}
      <li class="publication-item">
        <span class="publication-title">{{ pub.title }}</span><br />
        <span class="publication-meta">{{ pub.authors }}. {{ pub.venue }}.</span>
        {% if pub.link and pub.link != "" and pub.link != "#" %}
          <br /><a href="{{ pub.link }}">Link</a>
        {% endif %}
      </li>
      {% endfor %}
    </ul>
    {% endfor %}
  </section>
</div>
