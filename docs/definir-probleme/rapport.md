---
layout: default
---

{% assign pages = site.pages | sort: "order" %}
{% for page in pages %}
 {% if page.expose == "Définir le problème" %}
    {{- page.content | markdownify -}}
  {% endif %}
{% endfor %}