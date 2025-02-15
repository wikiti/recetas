---
layout: default
title: Mis recetas
---

# Mis recetas

Ésta es la lista de recetas que he ido recopilando a lo largo de los años.

{% for recipe in site.recipes %}

- [{{ recipe.title }}]({{ recipe.url }})

{% endfor %}
