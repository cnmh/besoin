---
layout: presentation
order: 7
---

{% assign pages = site.pages | sort: "order" %}
{% for page in pages %}
{% if page.expose == "empathie assistant dentaire" %}

<!-- page.content | markdownify -->
{{page.content }}

{% endif %}
{% endfor %}
