---
layout: default
title: "debugging js.erb files"
description: ""
category: 
tags: []
---
I've been doing a lot of unobtrusive Javascript / AJAX stuff in Rails reccently and I'm often coming across the situation where there is an error in my js.erb javascript code, which prevents it
being rendered as per the explanation that Steve gives here http://www.alfajango.com/blog/rails-js-erb-remote-response-not-executing/

His advice works, however, I mostly use Chrome when developing so here are the equivalent instructions 

Go to Developer Tools
Settings (bottom right corner) > General > Console
Tick Log XMLHttpRequests

Refresh the page you're having trouble with and complete an action that will call the js.erb file you're having trouble with
Click on the relevant XHR finished loading: [link]
This will open up the Network tab where you can see your ajax request. 
Clicking on the relevant AJAX request will open up more info about it. Go to the Response tab. 
Copy the javascript from the response tab. 
Navigate to the Console tab
Past in your copied javascript
Press return
Errors will be found and gifted to you in lovely red writing. 


