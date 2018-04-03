---
title: About
date: 2018-04-03 06:18:35 Z
hosts:
- name: Tomas Lau
  twitter: tomaslau
  image: "/uploads/2018/04/03/x1RsGCyH_400x400.jpg"
- name: Dustin Delatore
  twitter: whos_dustin
  image: ''
layout: about
---

<div class="about">
  {% for host in page.hosts %}

  <div class="cell">
    <img class="img-album" src="{{ host.image | relative_ur }}" alt="{{ host.name }}">
    <h3>{{ host.name }}</h3>
    <a class="badge" href="https://twitter.com/{{ host.twitter }}" title="Follow {{ host.name }} on Twitter">
      <i data-feather="twitter" aria-hidden="true"></i>
      {{ host.twitter | prepend: '@'}}
    </a>
  </div>

  {% endfor %}
</div>