---
layout: page
title: "Guides"
permalink: /guides/
---
<ul>
{% for guide in site.guides %}
  <li>
    <a href="{{ guide.url | absolute_url }}"> {{ guide.name }}</a>
  {{ guide.excerpt }}
  </li>	
{% endfor %}
</ul>