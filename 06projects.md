---
layout: page
title: Projects
permalink: /projects/ 
---
<div id="posts">
  <ul>
    {% for post in site.posts %}
	{% if post.category == "projects" %}
      <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> by <span class="italic">{{ post.author }}</span></li>
	{% endif %}    
{% endfor %}
  </ul>
</div>
