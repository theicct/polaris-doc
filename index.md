---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: Polaris Model Documentation
---

The ICCT's Polaris model is a Python-based, global maritime emissions projection model covering all ocean transport activity.

It was first developed in 2022-23 by Gabe Alvarez, Sola Zheng, Francielle Carvalho, Jakob Schmidt, Erik Pronk, Bryan Comer, and Josh Miller.


## Versions

Polaris is under continuing development. Documentation of all versions since v0.0.0 can be found here.

{% assign pages = site.pages | sort: "title" | reverse %}
{% for page in pages %}
{% if page.dir contains '/versions/' and page.title contains 'Polaris v'%}
<li><a class="page-link" href="{{ page.url | relative_url }}">{{ page.title | escape }}</a></li>
{% endif %}
{% endfor %}
