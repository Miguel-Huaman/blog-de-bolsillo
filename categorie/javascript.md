---
title: "Categoría: 'JavaScript'"
categories: javascript
layout: basic
description: "Todos los posts de la categoría: 'JavaScript'."
---

<h1>{{ page.title }}</h1>

{% for item in site.articulos reversed%}
{% for categorie in item.categories %}
{% if categorie contains "javascript" %}
<ul>
    {% include list-date-tag.html %}
</ul>
{% endif %}
{% endfor %}
{% endfor %}
