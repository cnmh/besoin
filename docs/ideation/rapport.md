---
layout: default
---

{% assign pages = site.pages | sort: "order" %}
{% for page in pages %}
 {% if page.expose == "Idéation" %}
    {{- page.content | markdownify -}}
  {% endif %}
{% endfor %}