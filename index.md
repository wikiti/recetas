# Mis recetas

{% assign recipes = site.pages | where: "path", "recipes" %}
{% for recipe in recipes %}
- [{{ recipe.title }}]({{ recipe.url }})
{% endfor %}
