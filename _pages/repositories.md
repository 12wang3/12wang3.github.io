---
layout: page
permalink: /repositories/
title: Repositories
description: "Follow me on GitHub: <a href='https://github.com/12wang3'>https://github.com/12wang3</a>"
nav: true
nav_order: 3
---
<!-- Follow me on GitHub: [https://github.com/12wang3](https://github.com/12wang3)

--- -->

## GitHub users

{% if site.data.repositories.github_users %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.html username=user %}
  {% endfor %}
</div>
{% endif %}

---

## GitHub Repositories

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}
