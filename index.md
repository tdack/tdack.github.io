---
layout: default
title: Repositories
---
{% for repository in site.github.public_repositories %}
* [{{ repository.name }}]({% if repository.homepage %}{{ repository.homepage }}{% else %}{{ repository.html_url }}{% endif %}) - {{ repository.description }}
{% endfor %}
