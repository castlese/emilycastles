---
layout: default
title: Page Title
pagetitle: Page <TITLE>
description: Page <DESCRIPTION>
---


<div id="home">

    {% for post in site.posts %}
      <div>
        <h2 a href="{{ post.url }}">{{ post.title }}</h2>
        <h4>{{ post.date | date_to_string }}</h4>
        <p>{{ post.description }}</p>
      </div>
    {% endfor %}

</div>