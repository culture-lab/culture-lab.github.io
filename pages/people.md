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
<div class="row t10">
    {% for post in site.categories.people_PROF %}
    <a class="medium-4 columns b30" style="float:left;position:static" href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">    
    <img src="https://culture-lab.github.io/images/{{post.image.title}}" style="width:150px;height:150px;">
    <br>{{ post.title }}</a>
    {% endfor %}
  </div>


<br>
## 박사
<div class="row t10">
    {% for post in site.categories.people_PHD %}
    <a class="medium-4 columns b30" style="float:left;position:static" href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">    
    <img src="https://culture-lab.github.io/images/{{post.image.title}}" style="width:150px;height:150px;">
    <br>{{ post.title }}</a>
    {% endfor %}
  </div>


<br>
## 석사

<div class="row t10">
    {% for post in site.categories.people_MA %}
    <a class="medium-4 columns b30" style="float:left;position:static" href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">    
    <img src="https://culture-lab.github.io/images/{{post.image.title}}" style="width:150px;height:150px;">
    <br>{{ post.title }}</a>
    {% endfor %}
  </div>
