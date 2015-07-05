---
layout: default
title: Troy Dack's GitHub Projects
---

{% for repository in site.github.public_repositories %}
  * [{{ repository.name }}] ({% if repsository.url %}{{ repository.url }}{% else %}repository.html_url{% endif %})
{% endfor %}
