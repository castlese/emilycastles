---
layout: default
title: "pretty excited that I just used recursion in real life"
description: ""
category: 
tags: []
---
Rails Employee model - when change the display order of one employee, need to change the display order for all employees below that on the list
class Employee < ActiveRecord::Base
	before_validation :set_display_order 

  validates_presence_of :first_name, :last_name, :store_id, :display_order

  def is_last
    display_order == Employee.order("display_order DESC").first.display_order
  end

  def set_display_order
    if self.new_record?
      set_display_order_of_new_record     
    else
      set_display_order_after_update
    end
  end

private

  def set_display_order_of_new_record
    if Employee.all.count == 0
        self.display_order = 1
    else
      last_employee = Employee.order("display_order DESC").first
      self.display_order = last_employee.display_order + 1
    end
  end  

  def set_display_order_after_update
    if self.display_order_changed? && !self.is_last
      order = display_order
      next_employee = Employee.find_by_display_order(order)

      #recursively updates display order for all records with display_order > order
      next_employee.update_attributes(:display_order => (order + 1))
    end
  end   


end

