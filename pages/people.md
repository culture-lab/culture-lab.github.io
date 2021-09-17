---
layout: page
show_meta: false
title: "연구실 구성원"
subheadline: "Participants"
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/people/"
---
<ul>
    {% for post in site.categories.design %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
