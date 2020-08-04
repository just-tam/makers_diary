# Makers Day 5 - 24th July 2020
#ruby

_Things I have learned today_

For Chapter 6 - quiz1

Set a state for cave to use as a second conditions

``` ruby
cave = false

while true do
  move = gets.chomp
  if move == "north"
    if cave == false
      puts "You are in a scary cave."
      cave = true
    elsif cave == true
      puts "You walk into sunlight."
      break
    end
  elsif move == "south"
    puts "You are in a scary passage."
    cave = false
  end
end
```

