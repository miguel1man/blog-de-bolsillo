---
title: "Tag: 'HTML'"
tag: html
layout: basic
description: "Todos los posts con el tag: 'HTML'."
---

<h1>{{ page.title }}</h1>

{% for item in site.articulos reversed%}
{% for tag in item.tags %}
{% if tag contains "html" %}
<ul>
    {% include list-date-tag.html %}
</ul>
{% endif %}
{% endfor %}
{% endfor %}