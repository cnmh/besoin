---
layout: default
---

{% assign pages = site.pages | sort: "order" %}
{% for page in pages %}
{% if page.expose == "empathie-psychomotricien" && page.expose == "Resumer" %}
{{- page.content | markdownify -}}
{% endif %}
{% endfor %}
