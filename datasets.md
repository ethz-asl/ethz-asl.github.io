---
layout: dataset
title: "ASL Datasets"
permalink: /datasets/
---

# ASL Datasets

This page lists datasets recorded at the Autonomous Systems Lab.
The actual data files are hosted on the ETH Research Collection and other long-term repositories.

<div class="dataset-grid">
  {%- assign datasets = site.datasets | sort: "year" | reverse -%}

  {%- for dataset in datasets -%}
    {%- assign is_featured = dataset.featured | default: false -%}
    {%- if dataset.important and dataset.important == true -%}
      {%- assign is_featured = true -%}
    {%- endif -%}

    <article class="dataset-card{% if is_featured %} dataset-card--featured{% endif %}">
      <h2 class="dataset-card__title">
        {%- if is_featured -%}
          <span class="dataset-card__star" aria-label="Featured dataset" title="Featured dataset">★</span>
        {%- endif -%}
        <a href="{{ dataset.url | relative_url }}">
          {{ dataset.title }}
        </a>
      </h2>

      <p class="dataset-card__meta">
        {%- if dataset.venue -%}
          <span class="dataset-card__venue">{{ dataset.venue }}</span>
        {%- endif -%}
        {%- if dataset.year -%}
          {%- if dataset.venue -%} • {%- endif -%}
          <span class="dataset-card__year">{{ dataset.year }}</span>
        {%- endif -%}
      </p>

      {%- if dataset.description -%}
        <p class="dataset-card__description">
          {{ dataset.description }}
        </p>
      {%- endif -%}

      {%- if dataset.doi or dataset.data_url -%}
        <p class="dataset-card__links">
          {%- if dataset.doi -%}
            <a href="{{ dataset.doi }}" class="dataset-card__link">Paper / DOI</a>
          {%- endif -%}
          {%- if dataset.data_url -%}
            {%- if dataset.doi -%} · {%- endif -%}
            <a href="{{ dataset.data_url }}" class="dataset-card__link">Download data</a>
          {%- endif -%}
        </p>
      {%- endif -%}
    </article>
  {%- endfor -%}
</div>

<style>
  .dataset-grid {
    display: flex;
    flex-direction: column;
    gap: 1.25rem;
    margin-top: 1rem;
  }

  @media (min-width: 800px) {
    .dataset-grid {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 1.5rem;
    }
  }

  .dataset-card {
    border: 1px solid #dddddd;
    border-radius: 8px;
    padding: 0.9rem 1rem;
    background: #ffffff;
  }

  .dataset-card--featured {
    border-color: #f1c40f;
    box-shadow: 0 0 0 1px rgba(241, 196, 15, 0.2);
    background: #fffdf4;
  }

  .dataset-card__title {
    font-size: 1.05rem;
    margin: 0 0 0.2rem;
    line-height: 1.3;
  }

  .dataset-card__title a {
    text-decoration: none;
  }

  .dataset-card__title a:hover,
  .dataset-card__title a:focus {
    text-decoration: underline;
  }

  .dataset-card__star {
    color: #f39c12;
    margin-right: 0.35rem;
    font-size: 0.95em;
  }

  .dataset-card__meta {
    margin: 0 0 0.4rem;
    font-size: 0.85rem;
    color: #555555;
  }

  .dataset-card__description {
    margin: 0 0 0.4rem;
    font-size: 0.9rem;
  }

  .dataset-card__links {
    margin: 0;
    font-size: 0.85rem;
  }

  .dataset-card__link {
    text-decoration: none;
  }

  .dataset-card__link:hover,
  .dataset-card__link:focus {
    text-decoration: underline;
  }
</style>