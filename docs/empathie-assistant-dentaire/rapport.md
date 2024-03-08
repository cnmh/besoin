---
layout: default
---

{% assign pages = site.pages | sort: "order" %}
{% for page in pages %}
 {% if page.expose == "empathie assistant dentaire" %}
    {{- page.content | markdownify -}}
  {% endif %}
{% endfor %}

