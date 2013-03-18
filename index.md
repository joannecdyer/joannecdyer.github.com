---
layout: default
title: Joanne Dyer
---

### About Me

Developer of Lumio, the illuminating iOS puzzle game. Previously worked as a software consultant, developing for companies like Cassidian and General Electric.


### Projects & Posts

<ul id="posts">
  {% for post in site.posts %}
  <li>
    <h5><a href="{{ post.url }}">{{ post.title }}</a></h5>
    <p>{{ post.summary }}</p>
    {% if post.screenshots %}
      {% for screenshot in post.screenshots %}
        <img class="small-screenshot" src="{{ screenshot }}" alt="Screenshot">
      {% endfor %}
    {% endif %}
  </li>
  {% endfor %}
</ul>