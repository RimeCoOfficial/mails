---
layout: default
title: Home
---


# Messages

`upload` folder is used to store attachments for drafting purpose only

<ul>
  {% assign pages_list = site.docs %}
  {% for node in pages_list %}
    {% if node.title != null %}
      {% if node.layout == "email" %}
        <li>
          <a href="{{ site.baseurl }}{{ node.url }}" target="_blank">↳</a>
          {{ node.title }}
        </li>
      {% endif %}
    {% endif %}
  {% endfor %}
</ul>

<a href="http://php-lb-2022216618.us-east-1.elb.amazonaws.com/open/campaign/newsletter/ead727ee6c2453405e2fe2070f4622df#_=_">Newsletters</a>
