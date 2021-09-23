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
<br>
<ul>
    {% for post in site.categories.people_PROF %}
    <li style="list-style-type: none;">
    <a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">    
    <img src="https://culture-lab.github.io/images/{{post.image.title}}" style="width:150px;height:150px;">
    <br>{{ post.title }}</a>
    </li>
    {% endfor %}
</ul>


<br>
## 박사
<br>
<ul>
    {% for post in site.categories.people_PHD %}
    <li style="list-style-type: none;">
    <a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">    
    <img src="https://culture-lab.github.io/images/{{post.image.title}}" style="width:150px;height:150px;">
    <br>{{ post.title }}</a>
    </li>
    {% endfor %}
</ul>


<br>
## 석사

<div class="row t10">
    {% for post in site.categories.people_MA %}
    <a class="medium-4 columns b20" display="flex"  align-items="stretch" href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">    
    <img src="https://culture-lab.github.io/images/{{post.image.title}}" style="width:150px;height:150px;">
    <br>{{ post.title }}</a>
    {% endfor %}
  </div>
