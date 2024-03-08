---
layout: default
---

{% assign pages = site.pages | sort: "order" %}
{% for page in pages %}
 {% if page.expose == "empathie-kinesitherapeute" %}
    {{- page.content | markdownify -}}
  {% endif %}
{% endfor %}
