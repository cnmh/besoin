---
layout: default
---

{% assign pages = site.pages | sort: "order" %}

{% for page in pages %}
{% if page.empathie == "empathie-assistant-dentaire" %}
<!-- page.content | markdownify -->
{{page.content }}

{% endif %}
{% endfor %}

