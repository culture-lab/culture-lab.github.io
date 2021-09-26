---
layout: page
show_meta: false
title: Table test
subheadline: People
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
