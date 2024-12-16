# Ruby Getter Method Bug

This repository demonstrates a subtle bug related to the use of getter methods in Ruby.  The issue arises from a misconception about how modifying the value returned by a getter method affects the underlying instance variable.

## Bug Description

The `bug.rb` file contains Ruby code that defines a class with a getter method.  While it appears that assigning a new value to the getter method will update the instance variable, it actually does not. This is because the getter method only returns the value of the instance variable; it doesn't provide a setter functionality.

## Solution

The `bugSolution.rb` file presents a corrected version of the code.  It explicitly includes a setter method (`value=`) to properly modify the instance variable.  This demonstrates the proper way to update the value of an instance variable via a class method.

This example highlights a common pitfall for developers new to Ruby's object-oriented features.  Understanding the distinction between getter methods and setter methods is critical for writing correct and predictable object-oriented code in Ruby.