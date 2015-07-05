---
layout: default
title: Troy Dack's GitHub Projects
---
{% for repository in site.github.public_repositories %}
* [{{ repository.name }}]({% if repository.homepage %}{{ repository.homepage }}{% else %}{{ repository.html_url }}{% endif %})
  {{ repository.homepage }} - {{ repository.description }}
{% endfor %}
