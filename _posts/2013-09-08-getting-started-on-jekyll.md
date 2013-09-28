---
layout: default
title: "Getting started on Jekyll"
description: "I've been threatening to start a small blog for ages - mostly for my own benefit to keep track of the things I learn along the way, things I need to refer to frequently and and mistakes I make. 
I also find that I go to lots of talks and events and would like to keep track of any small nuggets of knowledge I learn, links to slides etc. 

I've been wanting to try out nitrous.io for a while now and I figured this would be a great way to start. Nitrous is a service which provides a development environment
in the cloud (wow, I love that phrase so much!). You can set up a Rails, Node.js, Python/Django or Go box and access it from any browser, anywhere. It's great!"
category: 
tags: [jekyll, nitrous]
---
# {{page.title}}

{% for tag in page.tags %}
<li><span>{{ tag }}</li>
{% endfor %}

I've been threatening to start a small blog for ages - mostly for my own benefit to keep track of the things I learn along the way, things I need to refer to frequently and and mistakes I make. 
I also find that I go to lots of talks and events and would like to keep track of any small nuggets of knowledge I learn, links to slides etc. 

I've been wanting to try out nitrous.io for a while now and I figured this would be a great way to start. Nitrous is a service which provides a development environment
in the cloud (wow, I love that phrase so much!). You can set up a Rails, Node.js, Python/Django or Go box and access it from any browser, anywhere. It's great!

I think it's going to be particularly useful for this site as I've decided to run it using Jekyll - which means instead of having a CMS to update blog posts and content, 
the content is written statically. This is particularly useful for a developer as I feel Wordpress and other equivalents would be way too heavy for my needs given that I 
can edit the code relatively quickly.

Setting up nitrous is really easy, just go to <a href="http://nitrous.io">notrous.io</a> and follow the instructions on there. I set up a small rails box - with just 768MB
of RAM and 1000MB of storage. That's fine for now. It works really quickly and I can always pay for more memory if needed. Link the box with your github and you'll be able to 
push your project to your remote github repository. 

Jekyll was also pretty easy to set up. I haven't used markdown or liquid formats before so I'll have a bit to play around with there but it doesn't look all that hard

Instead of manually adding new blog post files, I've gone with the suggestion of <a href="http://yeswejekyll.com">yeswejekyll.com</a> and have included a rake task to create new posts:

rake post title="A Title" [date="2012-02-09"] [tags=[tag1, tag2]]

Mostly the hard part for me is deciding on colours, fonts and styles - I get lost in that stuff so
