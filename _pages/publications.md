---
layout: archive
permalink: /publications/
title: "Highlighted Publications"
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can find all my publications on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
