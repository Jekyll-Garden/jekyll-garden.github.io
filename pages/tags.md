---
layout: Post
title: By Tags
permalink: /tags/
content-type: eg
---


<br>
<div>
{% assign tags =  site.notes | map: 'tags' | uniq %}
{% for tag in tags %}
  <h3>{{ tag }}</h3>
  <ul>
  {% for note in site.notes %}
    {% if note.tags contains tag %}
    <li><a href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a></li>
    {% endif %}
  {% endfor %}
  </ul>
{% endfor %}
</div>
<br/>
<br/>
