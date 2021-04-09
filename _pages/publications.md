---
layout: archive
title: "Publications"
header:
  # overlay_image: light.jpg
  # caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
  overlay_filter: rgba(0, 0, 0, .5)
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

Preprints
===

{% for post in site.preprints reversed %}
  {% include archive-single.html %}
{% endfor %}

