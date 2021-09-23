---
layout: page
show_meta: false
title: "연구실 구성원"
subheadline: "Participants"
header: no
permalink: "/people/"
---

## 교수
<div class="row t10">
    {% for post in site.categories.people_PROF %}
    <div class="medium-4 columns" style="float:left; width:200px;height:200px;">
      <a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">    
        <img src="https://culture-lab.github.io/images/{{post.image.title}}" style="width:150px;height:150px;">
        <br>{{ post.title }}
      </a>
    </div>
    {% endfor %}
  </div>


<br>
## 박사
<div class="row t10">
    {% for post in site.categories.people_PHD %}
    <div class="medium-4 columns" style="float:left; width:200px;height:200px;">
      <a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">    
        <img src="https://culture-lab.github.io/images/{{post.image.title}}" style="width:150px;height:150px;">
        <br>{{ post.title }}
      </a>
    </div>
    {% endfor %}
  </div>


<br>
## 석사

<div class="row t10">
    {% for post in site.categories.people_MA %}
    <div class="medium-4 columns" style="float:left; width:200px;height:200px;">
      <a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">    
        <img src="https://culture-lab.github.io/images/{{post.image.title}}" style="width:150px;height:150px;">
        <br>{{ post.title }}
      </a>
    </div>
    {% endfor %}
  </div>
