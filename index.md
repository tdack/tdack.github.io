---
layout: default
title: Troy Dack's GitHub Projects
---

{% for repository in site.github.public_repositories %}
  * [{{ repository.name }}]({{ repository.html_url }})
{% endfor %}
