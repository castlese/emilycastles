---
layout: default
title: Page Title
pagetitle: Emily Castles Rails Developer
description: home
---


<div id="home">

    {% for post in site.posts %}
      <div class="post">
        <h4 class="date">{{ post.date | date_to_string }}</h4>
        <h2 class="title"><a href="{{ post.url }}">{{ post.title }}</a></h2>
        
        <p>{{ post.description }}</p>
      </div>
    {% endfor %}

</div>