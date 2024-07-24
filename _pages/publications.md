---
layout: archive
permalink: /publications/
title: "Publications"
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% publications -f papers -q @*[year={{y}}]* %}
{% endfor %}
