---
layout: default
---

{% assign pages = site.pages | sort: "order" %}
{% for page in pages %}
 {% if page.empathie == "empathie-kinesitherapeute" %}
    {{- page.content | markdownify -}}
  {% endif %}
{% endfor %}
