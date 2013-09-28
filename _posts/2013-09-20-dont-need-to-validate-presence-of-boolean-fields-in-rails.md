---
layout: default
title: "don't need to validate presence of boolean fields in rails"
description: ""
category: 
tags: []
---
http://stackoverflow.com/questions/5170008/rails-validating-inclusion-of-a-boolean-fails-tests

migration

  def change
    -add a column which is always true/false but defaults to true
    add_column :table_name, :column name, :boolean, :default => 1
  end
  
model




see it's blank, no validation required. Specifically don't validate_presence_of OR validates :inclusion => (true, false)....
