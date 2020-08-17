# About Mocking
#ruby #mocks #mocking #doubles #stubs

[How to Use RSpec Mocks (Step-By-Step Tutorial) - RubyGuides](https://www.rubyguides.com/2018/10/rspec-mocks/)

### What is mocking?

You use mocks to test the interaction between two objects. Instead of testing the output value, like in a regular expectation.

### Why do we use mocking?

* Faking some external action like sending emails
* E.g. if you were testing a method that sends out a confirmation email
* When a class has a dependency on another class
* Stops tests from failing if there there is an issue with the dependent class, e.g. Airplane from Airport

### When to use mocks?

1. If the method under test returns a value & it has no side effects (creating files, making API requests, etc.) then you don’t need a mock. Just check for the return value.
2. If the method is working with external objects & sending orders to them, then you can mock the interactions with these objects.
3. If the method is REQUESTING data from an external service (like an API), then you can use a stub to provide this data for testing purposes.

You want to **reserve mocking for interactions with the outside world**.
In other words…

Avoid mocking your own application’s classes!

Why?

Because that promotes coupling your tests with implementation details & **it makes your code harder to change**.

The only exception is for classes that are wrappers for 3rd party code.

### Stubs

For Stubs we use ‘allow’ to create the behaviour before executing tests

### Mocks

For mocks we use ‘expect’ to predict the behaviour e.g. 

``` 
processor = double(‘processor’)

expect(processor).to receive(:flip)with(‘image.jpg)
```

The expectation is set before the code is run, because we are expecting the method to be run first.