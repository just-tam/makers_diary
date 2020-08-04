#  Makers Day 4 - 23rd July 2020
#ruby #maths

_Things I have learned today_

Fibonacci sequence - a series of numbers in which each number ( _Fibonacci number_ ) is the sum of the two preceding numbers. The simplest is the series 1, 1, 2, 3, 5, 8, etc.

Using a times loop to write a simple fib sequence:

``` ruby
num1 = 0
num2 = 1

20.times do
  puts num1
  num3 = num1 + num2
  num1 = num2
  num2 = num3
end
```

Adding together the sum of numbers between two numbers, e.g. 1 - 250:

``` ruby
number = 1
total = 0

while number < 251 do
  total += number
  number += 1
end

puts total
```

 **instantiation** - The process of asking classes to create instances

