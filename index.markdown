---
title: Gallery index
layout: index
---
<p>Famous movie scenes from Harry Potter filmed in London </p>
<p style="color: #800080;">“Harry Potter and the Order of the Phoenix” —— London</p>
<div id = "gallery">
  {% assign sorted_exhibits = site.exhibits | sort: "date" %}
  {% for exhibit in sorted_exhibits %}
    {% assign licence_url = site.data.licences | find: "licence", exhibit.licence %}
    {% assign creator = site.data.creators | find: "name", exhibit.creator %}
    <div class = "grid_cell">
      <a href = "{{ exhibit.url | relative_url }}"><img src="{{ exhibit.image-url }}" class="gallery_thumb"></a>
      <p class = "caption"><a href = "{{ exhibit.url | relative_url }}">{{ exhibit.title }}</a> by <a href = "{{ creator.homepage }}">{{ exhibit.creator }}</a></p>
      <p><a href="{{ licence_url.url }}">{{ exhibit.licence }}</a></p>
    </div>
  {% endfor %}
  
</div>

<p style="color: #800080;">“Mysterious Philosopher's Stone” —— London</p>
<div id = "gallery1">
  {% assign sorted_exhibits1 = site.exhibits1 | sort: "date" %}
  {% for exhibit1 in sorted_exhibits1 %}
    {% assign licence_url = site.data.licences | find: "licence", exhibit.licence %}
    {% assign creator = site.data.creators | find: "name", exhibit1.creator %}
    <div class = "grid_cell">
      <a href = "{{ exhibit1.url | relative_url }}"><img src="{{ exhibit1.image-url }}" class="gallery_thumb"></a>
      <p class = "caption"><a href = "{{ exhibit1.url | relative_url }}">{{ exhibit1.title }}</a> by <a href = "{{ creator.homepage }}">{{ exhibit1.creator }}</a></p>
      <p><a href="{{ licence_url.url }}">{{ exhibit1.licence }}</a></p>
    </div>
  {% endfor %}
  
</div>

<p style="color: #800080;">“Harry Potter and the Prisoner of Azkaban” —— London</p>
<div id = "gallery2">
  {% assign sorted_exhibits1 = site.exhibits2 | sort: "date" %}
  {% for exhibit1 in sorted_exhibits1 %}
    {% assign licence_url = site.data.licences | find: "licence", exhibit.licence %}
    {% assign creator = site.data.creators | find: "name", exhibit1.creator %}
    <div class = "grid_cell">
      <a href = "{{ exhibit1.url | relative_url }}"><img src="{{ exhibit1.image-url }}" class="gallery_thumb"></a>
      <p class = "caption"><a href = "{{ exhibit1.url | relative_url }}">{{ exhibit1.title }}</a> by <a href = "{{ creator.homepage }}">{{ exhibit1.creator }}</a></p>
      <p><a href="{{ licence_url.url }}">{{ exhibit1.licence }}</a></p>
    </div>
  {% endfor %}
  
</div>
