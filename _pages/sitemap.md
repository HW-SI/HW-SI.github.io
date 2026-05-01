---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

Main pages on this website. The XML sitemap is available at [sitemap.xml]({{ base_path }}/sitemap.xml).

<h2>Pages</h2>
{% assign visible_pages = site.pages | where_exp: "page", "page.title != nil" | sort: "title" %}
{% for post in visible_pages %}
  {% include archive-single.html %}
{% endfor %}
