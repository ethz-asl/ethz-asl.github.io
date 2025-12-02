---
layout: default
title: ASL Datasets
permalink: /datasets/
---

{%- assign datasets = site.datasets | sort: "year" | reverse -%}

# ASL Datasets

This page lists datasets recorded at the Autonomous Systems Lab.
The actual data files are hosted on the ETH Research Collection and other long-term repositories.

<div class="dataset-table-wrapper">
  <table class="dataset-table">
    <thead>
      <tr>
        <th class="dt-year">Year</th>
        <th class="dt-title">Dataset</th>
        <th class="dt-links">Links</th>
      </tr>
    </thead>
    <tbody>
      {%- for dataset in datasets -%}
        {%- assign is_featured = dataset.featured | default: false -%}
        {%- if dataset.important and dataset.important == true -%}
          {%- assign is_featured = true -%}
        {%- endif -%}

        <tr class="dataset-row{% if is_featured %} dataset-row--featured{% endif %}">
          <td class="dt-year">
            {%- if dataset.year -%}{{ dataset.year }}{%- endif -%}
          </td>

          <td class="dt-title">
            {%- if is_featured -%}
              <span class="dt-star" aria-label="Featured dataset" title="Featured dataset">★</span>
            {%- endif -%}
            <a href="{{ dataset.url | relative_url }}">
              {{ dataset.title }}
            </a>
            {%- if dataset.description -%}
              <span class="dt-description">
                — {{ dataset.description | strip_newlines }}
              </span>
            {%- endif -%}
          </td>

          <td class="dt-links">
            {%- if dataset.doi -%}
              <a href="{{ dataset.doi }}">DOI</a>
            {%- endif -%}
            {%- if dataset.data_url -%}
              {%- if dataset.doi -%} · {%- endif -%}
              <a href="{{ dataset.data_url }}">Data</a>
            {%- endif -%}
          </td>
        </tr>
      {%- endfor -%}
    </tbody>
  </table>
</div>

<style>
  .dataset-table-wrapper {
    margin-top: 1rem;
    font-size: 0.9rem;
  }

  .dataset-table {
    width: 100%;
    border-collapse: collapse;
  }

  .dataset-table thead th {
    text-align: left;
    font-weight: 600;
    padding: 0.25rem 0.4rem;
    border-bottom: 1.5px solid #000000; /* top rule (header) */
    border-top: 1.5px solid #000000; /* bottom rule (header) */
    font-size: 0.85rem;
  }

  .dataset-table tbody td {
    padding: 0.18rem 0.4rem;
    border-top: 0.5px solid #cccccc; /* thin horizontal rules between rows */
    vertical-align: top;
  }

  .dataset-table tbody tr:last-child td {
    border-bottom: 1.5px solid #000000; /* bottom rule like IEEE tables */
  }

  .dt-year {
    white-space: nowrap;
    font-variant-numeric: tabular-nums;
    width: 3.2rem;
  }

  .dt-links {
    white-space: nowrap;
  }

  .dt-title a {
    font-weight: 500;
  }

  .dt-title a:hover,
  .dt-title a:focus {
    text-decoration: underline;
  }

  .dt-description {
    color: #555555;
  }

  /* Featured row styling: keeps the fun star + yellow, but table-ish */
  .dataset-row--featured {
    background: #fffbe8;
    box-shadow: inset 0 0 0 1px #f1c40f;
  }

  .dt-star {
    color: #e39b00;
    margin-right: 0.3rem;
    font-size: 0.9em;
  }
</style>
