---
layout: page
title: Paper
---
{% include JB/setup %}

####Main Publication
<ul id='tag_list'>
{% for tag in site.tags %}
<li class='tag_item' id='{{ tag[0]  }}'>
<span class='tag_name'>{{ tag[0]  }}</span>
<span>
<ul>

{% for post in tag[1] %}
<li class='tag_post'><a href="{{ BASE_PATH }}{{ post.url  }}" title="{{ post.title  }}">{{ post.title  }}</a></li>
{% endfor %}
</ul>
</span>
</li>
{% endfor %}
</ul>
 
<script src="{{ BASE_PATH }}/assets/js/jquery-1.11.1.min.js" type="text/javascript" charset="utf-8"></script>
<script src="{{ BASE_PATH }}/assets/js/jquery.tagcloud.js" type="text/javascript" charset="utf-8"></script>
<script language="javascript">
$.fn.tagcloud.defaults = {
size: {start: 0.9, end: 2, unit: 'em'},
color: {start: '#e77471', end: '#f62817'}
};
 
$(function () {
$('#tag_cloud a').tagcloud();
});
</script>
