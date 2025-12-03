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
              <a href="/{{ dataset.doi }}">DOI</a>
            {%- endif -%}
          </td>
        </tr>
      {%- endfor -%}
    </tbody>
  </table>
</div>

<style>
/* === ASL dataset table: LaTeX / IEEE style === */

.dataset-table-wrapper {
  margin-top: 1rem;
  font-size: 0.9rem;
}

.dataset-table {
  width: 100%;
  border-collapse: collapse;
  border-top: 1.5px solid #000;      /* top rule */
}

/* Header row */
.dataset-table thead th {
  padding: 0.25rem 0.6rem 0.2rem;
  font-weight: 600;
  font-size: 0.9rem;
  text-align: left;
  border-bottom: 1.5px solid #000;   /* heavy rule under header */
}

/* Body cells */
.dataset-table tbody td {
  padding: 0.18rem 0.6rem 0.12rem;
  vertical-align: baseline;
  border: none;                      /* no per-row rules (like LaTeX) */
}

/* Bottom rule of table */
.dataset-table tbody tr:last-child td {
  border-bottom: 1.5px solid #000;
}

/* Column tweaks */
.dt-year {
  white-space: nowrap;
  font-variant-numeric: tabular-nums;
  width: 3.2rem;
}

.dt-links {
  white-space: nowrap;
  text-align: right;
}

.dt-title a {
  font-weight: 500;
}

.dt-title a:hover,
.dt-title a:focus {
  text-decoration: underline;
}

.dt-description {
  color: #555;
}

/* Featured rows: keep yellow highlight + box, but subtle */
.dataset-row--featured {
  background: #fffbe8;
  box-shadow: inset 0 0 0 1px #f1c40f;
}

.dt-star {
  color: #e39b00;
  margin-right: 0.35rem;
  font-size: 0.9em;
}

/* Light horizontal separators (IEEE-ish but slightly modern) */
.dataset-table tbody tr {
  border-bottom: 0.6px solid #ddd;   /* subtle, barely visible */
}

.dataset-table tbody tr:last-child {
  border-bottom: 1.5px solid #000;   /* keep heavy final rule */
}

.dataset-table thead th {
  border-bottom: 2.5px solid #000;   /* thicker IEEE-style header rule */
}


</style>
