---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: Post
permalink: /
title: Jekyll Garden
---

<div>
  <h3>{{ site.heading }}</h3>
  <p>A brief description of your site</p>
  <p>A longer bio about yourself and what you do.</p>
  
  <div>
    <a href="mailto:{{ site.email }}" class="btn">Get in touch</a>
    <a href="{{ site.baseurl }}/notes" class="btn">View Notes</a>
  </div>
</div>

<div class="card-grid">
  <div class="card">
    <h4><a href="{{ site.baseurl }}/notes">Working Notes <span class="arrow">→</span></a></h4>
    <p>Ongoing thoughts and ideas.</p>
  </div>
  <div class="card">
    <h4><a href="{{ site.baseurl }}/about">About <span class="arrow">→</span></a></h4>
    <p>Learn more about me.</p>
  </div>
</div>