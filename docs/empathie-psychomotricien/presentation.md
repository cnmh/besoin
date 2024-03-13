---
layout: presentation
order: 1
---

{% assign pages = site.pages | sort: "order" %}
{% for page in pages %}
 {% if page.empathie == "empathie-psychomotricien" %}
    {{- page.content | markdownify -}}
  {% endif %}
{% endfor %}