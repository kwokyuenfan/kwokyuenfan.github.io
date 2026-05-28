---
layout: page
permalink: /publications/
title: publications
description: Publications in peer-reviewed journals.
nav: true
nav_order: 2
bib_search: true
---
<!-- _pages/publications.md -->
<div class="publications">
{%- if site.enable_bib_search %}
  <div class="search-bar">
    <div class="search-table">
      <div class="search-cell">
        <i class="fa-solid fa-search"></i>
        <input
          id="bibsearch"
          type="text"
          class="form-control"
          placeholder="Search publications..."
        />
      </div>
    </div>
  </div>
{%- endif %}
{% bibliography --file papers %}
</div>
