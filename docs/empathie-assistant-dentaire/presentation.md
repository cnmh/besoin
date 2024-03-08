---
layout: presentation
order: 1
---

{% assign pages = site.pages | sort: "order" %}
{% for page in pages %}
 {% if page.expose == "empathie avec assistant dentaire médecin spécialiste Interne" %}
    {{- page.content | markdownify -}}
  {% endif %}
{% endfor %}
