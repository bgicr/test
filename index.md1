---
layout: page
title: BGI Cancer Research
tagline: demo v0.1
---
{% include JB/setup %}


TODO:
    
    Add Group Information here.
    
    list:
	1. Who we are.
	2. What we do.
	3. What we have done.

    
###Core Members:

{% for category in site.categories %}
  <h4 id="{{ category[0]  }}-ref">{{ category[0] | join: "/"  }}</h4>
  <ul>
    {% assign pages_list = category[1] %}
    {% include JB/pages_list %}
  </ul>
{% endfor %}

