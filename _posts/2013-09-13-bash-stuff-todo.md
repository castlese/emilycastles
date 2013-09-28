---
layout: default
title: "bash stuff: TODO"
description: ""
category: 
tags: [bash]
---

<h3>Get Bash to run as default</h3>
  <p>I have tried chsh bash - says that bash is my default shell but aliases set in bash.rc are not working. Or any other scripts. 

  Works if I do </p>
  - bash
  - [alias command]
  
  Do I need to do this everytime??
  
<h3>project commands that start up all the right terminal tabs</h3>
  <p>eg: -cashanalyitics
    This will open up the following tabs:
      work/cashanalytics rails s (tab title Server)
      work/cashanaytics rake jobs:work (tab title Delayed Job
      work/cashanalytics guard (tab title Guard or Tests)
      work/cashanalytics rails c (tab title Console)
      work/cashanalytics (tab title Stuff - open terminal for things, github etc</p>
      pgadmin (opens up DBMS)
      open chrome on base.lvh.me:3000
      open sublime on folder cashanalytics
      
<h3>Show github branch on command line</h3>
http://code-worrier.com/blog/git-branch-in-bash-prompt/

<h3>git commit hook to run tests and performance tests</h3>
http://code-worrier.com/blog/git-branch-in-bash-prompt/