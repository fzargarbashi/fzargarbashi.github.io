---
layout: page
permalink: /gallery/
title: Gallery
description: A collection of my astro photos.
nav: true
nav_order: 2
---

<style>
  .gallery-intro {
    margin-bottom: 2rem;
  }

  .gallery-year {
    margin: 2.5rem 0 1.25rem;
    padding-bottom: 0.5rem;
    border-bottom: 1px solid var(--global-divider-color);
  }

  .gallery-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }

  .gallery-card {
    margin: 0;
    overflow: hidden;
    border: 1px solid var(--global-divider-color);
    border-radius: 0.75rem;
    background: var(--global-bg-color);
    box-shadow: 0 0.25rem 1rem rgba(0, 0, 0, 0.06);
    transition: transform 160ms ease, box-shadow 160ms ease;
  }

  .gallery-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 0.5rem 1.25rem rgba(0, 0, 0, 0.12);
  }

  .gallery-card a {
    display: block;
  }

  .gallery-card img {
    display: block;
    width: 100%;
    height: 240px;
    object-fit: cover;
  }

  .gallery-caption {
    padding: 0.9rem 1rem 1rem;
  }

  .gallery-caption h3 {
    margin: 0 0 0.35rem;
    font-size: 1.05rem;
  }

  .gallery-caption time {
    color: var(--global-text-color-light);
    font-size: 0.9rem;
  }

  .gallery-caption p {
    margin: 0.6rem 0 0;
    font-size: 0.95rem;
  }

  @media (prefers-reduced-motion: reduce) {
    .gallery-card {
      transition: none;
    }
  }

  @media (min-width: 601px) {
    .gallery-grid {
      grid-template-columns: repeat(2, minmax(0, 1fr));
    }
  }
</style>

{% assign gallery_years = site.data.gallery | group_by: 'year' %}
{% for year_group in gallery_years %}

<h2 class="gallery-year">{{ year_group.name }}</h2>
<div class="gallery-grid">
  {% for photo in year_group.items %}
  {% assign photo_path = photo.image | prepend: '/assets/img/gallery/' %}
  <figure class="gallery-card">
    <a href="{{ photo_path | relative_url }}">
      <img src="{{ photo_path | relative_url }}" alt="{{ photo.alt | escape }}" loading="lazy">
    </a>
    <figcaption class="gallery-caption">
      <h3>{{ photo.title }}</h3>
      <time datetime="{{ photo.date }}">{{ photo.date | date: '%-d %B %Y' }}{% if photo.location %}, {{ photo.location }}{% endif %}</time>
      {% if photo.description %}<p>{{ photo.description }}</p>{% endif %}
    </figcaption>
  </figure>
  {% endfor %}
</div>
{% endfor %}
