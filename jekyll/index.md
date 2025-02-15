# Mis recetas

{% assign recipes = site.pages | where: "path", "recetas" %}
{% for recipe in recipes %}
- [{{ recipe.title }}]({{ recipe.url }})
{% endfor %}
