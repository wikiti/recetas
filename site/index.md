---
layout: default
title: Mis recetas
---

# Mis recetas

Ésta es la lista de recetas que he ido recopilando a lo largo de los años:

{% for page in site.pages %}
    {% if page.url contains '/recetas/' %}
- [{{ page.title }}]({{ page.url }})
    {% endif %}
{% endfor %}

