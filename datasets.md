---
layout: default
title: ASL Datasets
permalink: /datasets/
---

# ASL Datasets

This page lists datasets recorded at the Autonomous Systems Lab.
The actual data files are hosted on the ETH Research Collection and other long-term repositories.

<div class="dataset-list">
  {%- assign datasets = site.datasets | sort: "year" | reverse -%}

  {%- for dataset in datasets -%}
    {%- assign is_featured = dataset.featured | default: false -%}
    {%- if dataset.important and dataset.important == true -%}
      {%- assign is_featured = true -%}
    {%- endif -%}

    <article class="dataset-row{% if is_featured %} dataset-row--featured{% endif %}">
      <span class="dataset-row__year">
        {%- if dataset.year -%}
          {{ dataset.year }}
        {%- endif -%}
      </span>

      <span class="dataset-row__text">
        {%- if is_featured -%}
          <span class="dataset-row__star" aria-label="Featured dataset" title="Featured dataset">★</span>
        {%- endif -%}

        <a href="{{ dataset.url | relative_url }}" class="dataset-row__title">
          {{ dataset.title }}
        </a>
      </span>
    </article>
  {%- endfor -%}
</div>

<style>
  .dataset-list {
    margin-top: 1rem;
    border-top: 1px solid #e0e0e0;
    font-size: 0.9rem;
  }

  .dataset-row {
    display: flex;
    align-items: baseline;
    padding: 0.25rem 0;
    border-bottom: 1px solid #f0f0f0;
  }

  .dataset-row__year {
    flex: 0 0 3.2rem; /* fixed year column */
    font-variant-numeric: tabular-nums;
    font-size: 0.8rem;
    color: #666666;
  }

  .dataset-row__text {
    flex: 1 1 auto;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    min-width: 0;
  }

  .dataset-row__title {
    text-decoration: none;
    font-weight: 500;
  }

  .dataset-row__title:hover,
  .dataset-row__title:focus {
    text-decoration: underline;
  }

  .dataset-row__meta,
  .dataset-row__description {
    margin-left: 0.25rem;
    color: #555555;
  }

  .dataset-row__star {
    color: #f39c12;
    margin-right: 0.25rem;
    font-size: 0.9em;
  }

  .dataset-row--featured {
    background: #fff7d6;
    border-left: 3px solid #f1c40f;
    padding-left: 0.5rem;
  }

</style>
