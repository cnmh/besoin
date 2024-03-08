---
layout: default
---

{% assign pages = site.pages | sort: "order" %}
{% for page in pages %}
 {% if page.expose =="Empathie avec infirmière de médecine général" %}
    {{- page.content | markdownify -}}
  {% endif %}
{% endfor %}
