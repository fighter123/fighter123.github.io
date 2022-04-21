---
title: archive
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
  {% assign sorted_exhibits2 = site.exhibits2 | sort: "date" %}
  {% for exhibit2 in sorted_exhibits2 %}
    {% assign licence_url = site.data.licences | find: "licence", exhibit2.licence %}
    {% assign creator = site.data.creators | find: "name", exhibit2.creator %}
    <div class = "grid_cell">
      <a href = "{{ exhibit2.url | relative_url }}"><img src="{{ exhibit2.image-url }}" class="gallery_thumb"></a>
      <p class = "caption"><a href = "{{ exhibit2.url | relative_url }}">{{ exhibit2.title }}</a> by <a href = "{{ creator.homepage }}">{{ exhibit2.creator }}</a></p>
      <p><a href="{{ licence_url.url }}">{{ exhibit2.licence }}</a></p>
    </div>
  {% endfor %}
  
</div>


<p style="color: #800080;">“Harry Potter and the Chamber of Secrets” —— London</p>
<div id = "gallery3">
  {% assign sorted_exhibits3 = site.exhibits3 | sort: "date" %}
  {% for exhibit3 in sorted_exhibits3 %}
    {% assign licence_url = site.data.licences | find: "licence", exhibit3.licence %}
    {% assign creator = site.data.creators | find: "name", exhibit3.creator %}
    <div class = "grid_cell">
      <a href = "{{ exhibit3.url | relative_url }}"><img src="{{ exhibit3.image-url }}" class="gallery_thumb"></a>
      <p class = "caption"><a href = "{{ exhibit3.url | relative_url }}">{{ exhibit3.title }}</a> by <a href = "{{ creator.homepage }}">{{ exhibit3.creator }}</a></p>
      <p><a href="{{ licence_url.url }}">{{ exhibit3.licence }}</a></p>
    </div>
  {% endfor %}
  
</div>

<p style="color: #800080;">“Harry Potter and the Deathly Hallows” —— London</p>
<div id = "gallery4">
  {% assign sorted_exhibits4 = site.exhibits4 | sort: "date" %}
  {% for exhibit4 in sorted_exhibits4 %}
    {% assign licence_url = site.data.licences | find: "licence", exhibit4.licence %}
    {% assign creator = site.data.creators | find: "name", exhibit4.creator %}
    <div class = "grid_cell">
      <a href = "{{ exhibit4.url | relative_url }}"><img src="{{ exhibit4.image-url }}" class="gallery_thumb"></a>
      <p class = "caption"><a href = "{{ exhibit4.url | relative_url }}">{{ exhibit4.title }}</a> by <a href = "{{ creator.homepage }}">{{ exhibit4.creator }}</a></p>
      <p><a href="{{ licence_url.url }}">{{ exhibit4.licence }}</a></p>
    </div>
  {% endfor %}
  
</div>

<p style="color: #800080;">“The Betrayal of the Half-Blood Prince” —— London</p>
<div id = "gallery5">
  {% assign sorted_exhibits5 = site.exhibits5 | sort: "date" %}
  {% for exhibit5 in sorted_exhibits5 %}
    {% assign licence_url = site.data.licences | find: "licence", exhibit5.licence %}
    {% assign creator = site.data.creators | find: "name", exhibit5.creator %}
    <div class = "grid_cell">
      <a href = "{{ exhibit5.url | relative_url }}"><img src="{{ exhibit5.image-url }}" class="gallery_thumb"></a>
      <p class = "caption"><a href = "{{ exhibit5.url | relative_url }}">{{ exhibit5.title }}</a> by <a href = "{{ creator.homepage }}">{{ exhibit5.creator }}</a></p>
      <p><a href="{{ licence_url.url }}">{{ exhibit5.licence }}</a></p>
    </div>
  {% endfor %}
  
</div>
