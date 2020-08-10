# About TDD (Test Driven Development)
#TDD #ruby

### *What is TDD?*

Test driven development is a software programming practice that can radically increase code quality and program design.

### *Why do we TDD*

Testing first can **minimise bugs and the need to refactor** as your codebase increases in size and complexity. **Starting off with well written and tested code can also save cost and time**.

### *When do we TDD?*

Tests can also serve as **documentation for your feature in an application**. Other developers on the team can read your tests and easily figure out what your code is looking to achieve.

By creating the tests first, you can ensure that the function that you are testing works the way it is intended to work and avoid any surprises further down the line.

### *How does TDD work?*

**Steps for TDD**

1. Write a failing test (RED)
2. Write _the simplest code possible_ to pass the test (GREEN)
3. Clean up (REFACTOR)
4. Repeat until all expectations have been specified.

**What is RSpec?**

RSpec is a DSL — Domain Specific Language testing framework written in Ruby to test Ruby code.

Initializing RSpec:

``` 
$ rspec --init
```

Running RSpec

``` 
$ rspec
```

**RSpec.describe** creates a test block for the example group, the space where you will put your tests.

### *Rules to follow:*

* Understand the specifications from the user story
* Identify the objects and behaviours you are testing
* Write your first test — and see it fail
* Write the simplest line of code to make that test pass
* Run the tests
* Refactor

### This is a common pattern which many of your unit tests will follow.

1. First you **arrange** all the preconditions required for your code to run - creating any objects and assigning any variables that you’re going to need.
2. Next, you **act**, or execute the code which needs to be run in order for your assertion to be true.
3. Finally, you **assert** that your action has had an effect, or that it returned the expected value.

### More TDD notes

**described_class** describes having access to _whatever thing_ was supplied to the **outermost** describe block as the argument, and let the author of the test to use that definition as-is without the magical subject behaviour attached.
