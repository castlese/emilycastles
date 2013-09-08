---
layout: post
title: "Getting started on Jekyll"
description: "This is my first post here. Been threatening to start a small blog for ages - to keep track of all the things I learn,"
category: 
tags: [jekyll, nitrous]
---
# {{page.title}}

{% for tag in page.tags %}
<li><span>{{ tag }}</li>
{% endfor %}

This is my first post here. Been threatening to start a small blog for ages - to keep track of all the things I learn, forget or screwed up along the way. 

Set up in nitrous.io - awesome!

As per http://yeswejekyll.com/ suggestions, I've included a rake task to create new posts here:

rake post title="A Title" [date="2012-02-09"] [tags=[tag1, tag2]]
