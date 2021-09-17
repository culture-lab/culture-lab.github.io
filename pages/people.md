---
layout: page
show_meta: false
title: "연구실 구성원"
subheadline: "Participants"
header:
   image_fullwidth: "header_unsplash_12.jpg"
permalink: "/people/"
---

<br>

## 교수
<ul>
    {% for post in site.categories.people_PROF %}
    <li style="list-style-type: none;">
    <a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">    
    <img src="https://culture-lab.github.io/images/{{post.image.title}}" style="width:100px;height:120px;">
    <br>{{ post.title }}</a>
    </li>
    {% endfor %}
</ul>


## 박사
<ul>
    {% for post in site.categories.people_DR %}
    <li>
    <img src="https://culture-lab.github.io/images/{{post.image.title}}" style="width:100px;height:120px;">
    <br>
    <a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>


## 석사
