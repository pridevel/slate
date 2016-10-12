---
title: API Reference

language_tabs:
  - shell
  - ruby
  - python
  - javascript

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/tripit/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true
---

# Ruby
 
## Introduction 

*Ruby is a powerful, flexible programming language you can use in web/Internet development, to process text, to create games, and as part of the popular Ruby on Rails web framework. Ruby is:

*High-level, meaning reading and writing Ruby is really easy—it looks a lot like regular English!

*Interpreted, meaning you don't need a compiler to write and run Ruby. You can write it on your own computer.
>The interpreter is the program that takes the code you write and runs it. You type code in the editor, the interpreter reads your code, and it shows you the result of running your code in the console. 

*Object-oriented, meaning it allows users to manipulate data structures called objects in order to build and execute programs. All you need to know is everything in Ruby is an object.

*Easy to use. Ruby was designed by Yukihiro Matsumoto (often just called "Matz") in 1995. Matz set out to design a language that emphasized human needs over those of the computer, which is why Ruby is so easy to pick up.


## Ruby's Basic DataTypes

* String 
 Strings are the words or phrases. You can define them in single quoutes(' ') or double quotes (" ").

```ruby
my_string = "Hello, World!"
 
my_other_string = 'What are you doing?'
```
* Number
 Ruby can handle both integers and floating point numbers (numbers with decimals).

```ruby
ten = 10
fifteen_point_two = 15.2
 
twenty_five_point_two = ten + fifteen_point_two;   
//output: 25.2

```
* Booleans
 The value of the boolean can be either true or false.
```ruby
 my_boolean = true
```
## Variable
* Variables are the letters or words that stores the single value. 

```ruby
 x = 20
```

## Maths
* You can perform mathematical operation like Addition (+), Subtraction (-), Division (/), Exponentiation (**),
Modulo (%),Multiplication (*) in Ruby.
* For example, 2**3 is 8, since 2**3 means "give me 2 * 2 * 2" (2 multiplied together 3 times). 3**2 is 9 (3 * 3), and so on.

Modulo returns the remainder of division. For example, 25 % 7 would be 4, since 7 goes into 25 3 times with 4 left over.

## Print and Puts Commamds
The **print** command just takes whatever you give it and prints it to the screen where as **puts** (for "put string") is slightly different: it adds a new (blank) line after the thing you want it to print.

```ruby
puts "heyyyyy"
puts 'Whatssupppp'

print "Hello!"
print "World!"

// output: heyyyyy
   Whatssupppp
   Hello!World!
```
## Methods on Strings
### .length 
 This method return the length of the string (that is, the number of characters—letters, numbers, spaces, and symbols).

```ruby
"hiee this is savi".length

// output: 17
```
<hr>
### .reverse 
 This method spits out a backwards version of the string you gave it.

```ruby
"hello savi".reverse

// output: "ivas olleh"
```
<hr>
### .upcase and .downcase
This methods are used to convert a string to ALL UPPER CASE or all lower case, respectively. 

```ruby
puts "savi".upcase

puts "savi".downcase

//output: SAVI
        savi
```
## Comments
### Single line Comments
 It is denoted by "#", in front of the line you want to comment out.

```ruby
    # this is comment.

```
<hr>
### Multi-Line Comment 
If you want to comment Multiple lines at a time you can use this method.
If you start with =begin and end with =end, everything between those two expressions will be a comment.

```ruby
=begin

heyy this is a command
this 
is '
another
comment 
=end

```
## Operators
* Ruby has three operators:  and (&&), or (||), and not (!)

### And(&&)
* It evaluates true when both the expressions are true.

TruthTable: 

true && true # => true,
true && false # => false,
false && true # => false,
false && false # => false

```ruby
# boolean_1 = 77 < 78 && 77 < 77
boolean_1 = false

# boolean_2 = true && 100 >= 100
boolean_2 = true

# boolean_3 = 2**3 == 8 && 3**2 == 9
boolean_3 = true
```
<hr>
### OR(||)
* it evaluates to true when one or the other or both expressions are true.

true || true # => true,
true || false # => true,
false || true # => true,
false || false # => false

```ruby

# boolean_1 = 2**3 != 3**2 || true
boolean_1 = true

# boolean_2 = false || -10 > -9
boolean_2 = false

# boolean_3 = false || false
boolean_3 = false

```
<hr>
### NOT(!)
* It makes true values false, and vice-versa.

!true # => false,
!false # => true

```ruby
# boolean_1 = !true
boolean_1 = false

# boolean_2 = !true && !true
boolean_2 = false
```

## Control Flow
### If statement
Ruby's **if** statement takes an expression, which is just a fancy word for something that has a value. If that expression is true, Ruby executes the block of code that follows the **if**.
If it's not true (that is, false), Ruby doesn't execute that block of code: it skips it and goes on to the next thing, that is **else** statement or **end**.
When you're done with your **if**, you have to tell Ruby by typing **end**.

If you want to add more options you can use **elsif** statement.

```ruby
age = 15

if age < 20
    print "you are young!!"
    
else
    
print "you have passed ur teenage"
end

output : you are young!!
```

```ruby
# elsif Example

x = 5, y = 4;

if x < y  
  puts "x is less than y!"
elsif x > y
  puts "x is greater than y!"
else
  puts "x equals y!"
end

```

##Loops 
Loops in Ruby are used to execute the same block of code a specified number of times. You can refer more about [loops](https://www.tutorialspoint.com/ruby/ruby_loops.htm) here.
### while loop

* This loop is used when you want to repeat an action in Ruby while a certain condition is true.

```ruby
counter = 1
while counter < 11
  puts counter
  counter = counter + 1
end

// output: 1 2 3 4 5 6 7 8 9 10
```
<hr>
### for loop

*This loop is used when you do know how many times you'll be looping.

```ruby
for i in 0..5
   puts "Value of local variable is #{i}"
end

// output:Value of local variable is 0
Value of local variable is 1
Value of local variable is 2
Value of local variable is 3
Value of local variable is 4
Value of local variable is 5
```

## Arrays

Arrays are collection of objects which are ordered and have index.
The index value starts from **0**.
Ruby arrays can hold objects such as String, Integer, Fixnum, Hash, Symbol, even other Array objects.
You can refere more about Arrays [here](https://ruby-doc.org/core-2.2.0/Array.html)

### Creating array

There are two ways to create an empty array:

1. my_arr = Array.new  => []
 
2. my_other_arr = []    => [] (Literal Method)

```ruby
my_arr = Array.new(10)
// this array has a length of 10 elements.


my_other_arr = [1, 2, "new", ["hie",5], 55, 100]; 

```
<hr>
### Displaying Elements of Array
Now we will see how to iterate through the elements of an Array. A more useful iterator is the **.each** method, which can apply an expression to each element of an object, one at a time. 
The syntax looks like this:

object.each { |item| # Do something }

You can also you below method if ypu don't want to use the '{ }'.

object.each do |item| 
  # Do something 
end

```ruby

Ex 1:
array = [1,2,3,4,5]

array.each do |x|
  x = x + 10
  puts "#{x}"
end

// output:  11
            12
            13
            14
            15

Ex 2:
nums = Array.new(10) { |e| e = e * 2 }

puts "#{nums}"

Output: [0, 2, 4, 6, 8, 10, 12, 14, 16, 18]
```
<hr>
### Accessing Element from Array
You can also access the single element from the array by specifying its **index**.
The first element gets index 0, the next gets index 1, the one after that gets index 2, and so on.

```ruby
// Accessing Element from Array Example
demo_array = [100, 200, 300, 400, 500]

print demo_array[2]

//output: 300

```
<hr>
### Adding Items to Array
Arrays are flexible because of the fact that we could easily add or remove an item or element from an Array.
For adding the element in an Array we use **.push** method. Push method inserts the element at the end of an array.

```ruby
// adding item into array
b = ["cat", 5, true]
b.push("dog")

// output: ["cat", 5, true, "dog"]
```

If you want to add value to the beginning of an array, you use the **unshift** method.
```ruby
b.unshift("8.53")
// output: ["8.53", "hello", 100, true, "dog"]
```
<hr>
### Removing Item From Array

To remove an element from array we use **pop** method.
This method removes an returns the element at the last item of an array.

```ruby
b.pop
Output: "dog"
array : ["8.53", "hello", 100, true]
```

To remove the first item, you use the shift method.
```ruby
b.shift
// Output: "6.23"
array : ["hello", 100, true]
 ```
<hr> 
### Replacing Item In Array

If we want to replace a specific item from an array we can do it as follows:

array : 
b = ["hello", 100, true]

b[1] = 50

// Output: b = ["hello", 50, true]

## Hash

A Hash is a collection of key-value pairs like this: "animal" => "tiger". 
It is similar to an Array, except that indexing is done via arbitrary keys of any object type, not an integer index.
Values are assigned to keys using "=>"
Hash syntax looks like this:

hash = {
  key1 => value1,
  key2 => value2,
  key3 => value3
}





 





















































