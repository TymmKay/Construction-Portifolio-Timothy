---
layout: layouts/base.njk
title: Projects
permalink: /projects/
---

# 🏗️ My Completed Projects

Here are some of my past construction and renovation projects:

{% for project in collections.projects %}
- [{{ project.data.title }}]({{ project.url }}) (Completed: {{ project.date | date: "%B %Y" }})
{% endfor %}
