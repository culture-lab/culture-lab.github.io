---
layout: page
subheadline: People
show_meta: false
title: Table test
teaser: "Communication, Seoul National University"
breadcrumb: true
tags:
    - post format
categories:
    - people_PHD
header: no

---
<!-- <ul>
    {% for post in site.categories.design %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul> -->


{% assign row = site.data.BTS[0] %}
{{ row | inspect }}


{% assign groups = site.data.BTS | group_by: "type" %}
<ul>
{% for g in groups %}
{% assign type = g.items | where: "type", "MV" %}
<li>name : {{ g.name }} {{ type.size }} type</li>
{% endfor %}
</ul>



<p> test updated 8900 </p>
<ul>
 {% for song in site.data.BTS %}
   {% if song.performer == "Agust D" %}
    <li>
        <a href={{song.URL}}>{{song.title}}</a>  {{song.view}}
  </li>
    {% endif %}
 {% endfor %}
</ul>


<table>
  {% for row in site.data.BTS %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>
