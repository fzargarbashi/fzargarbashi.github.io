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
    grid-template-columns: repeat(2, minmax(0, 1fr));
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

  @media (prefers-reduced-motion: reduce) {
    .gallery-card {
      transition: none;
    }
  }

  @media (max-width: 600px) {
    .gallery-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<p class="gallery-intro"></p>

<h2 class="gallery-year">2026</h2>
<div class="gallery-grid">
  <figure class="gallery-card">
    <a href="/assets/img/gallery/2026-02-24-M42-M43-OrionNebula.png">
      <img src="/assets/img/gallery/2026-02-24-M42-M43-OrionNebula.png" alt="Orion Nebula, M42 and M43" loading="lazy">
    </a>
    <figcaption class="gallery-caption">
      <h3>Orion Nebula (M42 &amp; M43)</h3>
      <time datetime="2026-02-24">24 February 2026, Zurich, Switzerland</time>
    </figcaption>
  </figure>

  <figure class="gallery-card">
    <a href="/assets/img/gallery/2026-02-24-Moon.png">
      <img src="/assets/img/gallery/2026-02-24-Moon.png" alt="The Moon" loading="lazy">
    </a>
    <figcaption class="gallery-caption">
      <h3>The Moon</h3>
      <time datetime="2026-02-24">24 February 2026, Zurich, Switzerland</time>
    </figcaption>
  </figure>
</div>

<h2 class="gallery-year">2025</h2>
<div class="gallery-grid">
  <figure class="gallery-card">
    <a href="/assets/img/gallery/2025-10-24-CometLemmon.png">
      <img src="/assets/img/gallery/2025-10-24-CometLemmon.png" alt="Comet Lemmon" loading="lazy">
    </a>
    <figcaption class="gallery-caption">
      <h3>Comet Lemmon</h3>
      <time datetime="2025-10-24">24 October 2025, S-Charl, Switzerland</time>
    </figcaption>
  </figure>

  <figure class="gallery-card">
    <a href="/assets/img/gallery/2025-10-24-Milkyway.png">
      <img src="/assets/img/gallery/2025-10-24-Milkyway.png" alt="The Milky Way" loading="lazy">
    </a>
    <figcaption class="gallery-caption">
      <h3>The Milky Way</h3>
      <time datetime="2025-10-24">24 October 2025, S-Charl, Switzerland</time>
    </figcaption>
  </figure>

  <figure class="gallery-card">
    <a href="/assets/img/gallery/2025-10-24-Mountain-SCharl-Switzerland.png">
      <img src="/assets/img/gallery/2025-10-24-Mountain-SCharl-Switzerland.png" alt="Mountain landscape in S-charl, Switzerland" loading="lazy">
    </a>
    <figcaption class="gallery-caption">
      <h3>A Night in the Alps</h3>
      <time datetime="2025-10-24">24 October 2025, S-Charl, Switzerland</time>
    </figcaption>
  </figure>

  <figure class="gallery-card">
    <a href="/assets/img/gallery/2025-08-08-Moon.png">
      <img src="/assets/img/gallery/2025-08-08-Moon.png" alt="The Moon" loading="lazy">
    </a>
    <figcaption class="gallery-caption">
      <h3>The Moon, Stacked</h3>
      <time datetime="2025-08-08">8 August 2025, Zurich, Switzerland</time>
    </figcaption>
  </figure>

  <figure class="gallery-card">
    <a href="/assets/img/gallery/2025-03-05-Moon.png">
      <img src="/assets/img/gallery/2025-03-05-Moon.png" alt="The Moon" loading="lazy">
    </a>
    <figcaption class="gallery-caption">
      <h3>Moon over a House</h3>
      <time datetime="2025-03-05">5 March 2025, Zurich, Switzerland</time>
    </figcaption>
  </figure>
</div>

<h2 class="gallery-year">2024</h2>
<div class="gallery-grid">
  <figure class="gallery-card">
    <a href="/assets/img/gallery/2024-12-16-M31-Andromeda%20Galaxy.png">
      <img src="/assets/img/gallery/2024-12-16-M31-Andromeda%20Galaxy.png" alt="Andromeda Galaxy, M31, and M110" loading="lazy">
    </a>
    <figcaption class="gallery-caption">
      <h3>Andromeda Galaxy (M31) &amp; M110</h3>
      <time datetime="2024-12-16">16 December 2024 · Zurich, Switzerland</time>
    </figcaption>
  </figure>

  <figure class="gallery-card">
    <a href="/assets/img/gallery/2024-12-16-M42-M43-OrionNebula.png">
      <img src="/assets/img/gallery/2024-12-16-M42-M43-OrionNebula.png" alt="Orion Nebula, M42 and M43" loading="lazy">
    </a>
    <figcaption class="gallery-caption">
      <h3>Orion Nebula (M42 &amp; M43)</h3>
      <time datetime="2024-12-16">16 December 2024 · Zurich, Switzerland</time>
    </figcaption>
  </figure>
</div>
