---
layout: default
title: Joanne Maynard
---

### About Me

Developer of TrackYourTV.com a website for keeping track of your favorite tv shows and Lumio an iOS puzzle game previously available on the App Store. Formerly worked as a software engineer contractor, developing for companies like Cassidian and General Electric.


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
    {% if post.large_screenshots %}
      {% for screenshot in post.large_screenshots %}
        <img class="large-screenshot" src="{{ screenshot }}" alt="Screenshot">
      {% endfor %}
    {% endif %}
  </li>
  {% endfor %}
</ul>
