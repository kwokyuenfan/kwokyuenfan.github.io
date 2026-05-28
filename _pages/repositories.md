---
layout: page
permalink: /repositories/
title: repositories
description: My GitHub repositories.
nav: true
nav_order: 4
---
<!-- _pages/repositories.md -->
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-baseline">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.liquid username=user %}
  {% endfor %}
</div>
<hr>
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-baseline">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
