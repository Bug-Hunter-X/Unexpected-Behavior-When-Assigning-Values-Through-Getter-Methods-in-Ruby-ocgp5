# Ruby Getter Method Assignment Bug

This repository demonstrates a subtle but common error in Ruby related to assigning values to instance variables through getter methods.

## The Bug
The `bug.rb` file contains a class (`MyClass`) with an instance variable `@value`.  Assigning a value to `my_instance.value` does not change the value of `@value` because no setter method is defined.  This leads to unexpected behavior where modifications don't persist.

## The Solution
The `bugSolution.rb` file demonstrates the solution. By explicitly defining a `value=` setter method, changes to the instance variable are correctly reflected.

## How to Reproduce
1. Clone this repository
2. Run `ruby bug.rb`
3. Observe that the value remains unchanged after the assignment.
4. Run `ruby bugSolution.rb`
5. Observe the corrected behavior with the explicit setter method.
