---
layout: default
title: Troy Dack's GitHub Projects
---
{% for repository in site.github.public_repositories %}
* [{{ repository.name }}]({% if repository.homepage = "" %}{{ repository.html_url }}{% else %}{{ repository.homepage }}{% endif %})
{{ repository.homepage }}
{% endfor %}
