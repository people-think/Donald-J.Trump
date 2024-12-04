---
layout: default
title: "People Think"
---

## Navigation

- {% for item in site.nav %}
  - [{{ item.title }}]({{ item.url }})
  {% if item.submenu %}
    - **Submenu:**
      {% for sub_item in item.submenu %}
        - [{{ sub_item.title }}]({{ sub_item.url }})
      {% endfor %}
  {% endif %}
{% endfor %}
