---
layout: default
title: Home
---

`upload` folder is used to store attachments for drafting purpose only

<ul>
  {% assign pages_list = site.docs %}
  {% for node in pages_list %}
    {% if node.title != null %}
      {% if node.layout == "email" %}
        <li>
          {{ node.title }}
          <a href="{{ site.baseurl }}{{ node.url }}" target="_blank">↳</a>
        </li>
      {% endif %}
    {% endif %}
  {% endfor %}
</ul>
