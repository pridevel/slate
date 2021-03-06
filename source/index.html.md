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

* Ruby is a powerful, flexible programming language you can use in web/Internet development, to process text, to create games, and as part of the popular Ruby on Rails web framework. Ruby is:

* High-level, meaning reading and writing Ruby is really easy—it looks a lot like regular English!

* Interpreted, meaning you don't need a compiler to write and run Ruby. You can write it on your own computer.
The interpreter is the program that takes the code you write and runs it. You type code in the editor, the interpreter reads your code, and it shows you the result of running your code in the console. 

* Object-oriented, meaning it allows users to manipulate data structures called objects in order to build and execute programs. All you need to know is everything in Ruby is an object.

* Easy to use. Ruby was designed by Yukihiro Matsumoto (often just called "Matz") in 1995. Matz set out to design a language that emphasized human needs over those of the computer, which is why Ruby is so easy to pick up.


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
* They are the labels for a piece of memory where we store our data such as objects, arrays, numbers, strings, etc.
* We can aslo assign one variable to other variable.

```ruby
 x = 20
 puts x
 
 output: 20
```

* With variables we can do something called string interplation, which means we can insert variables inside a string.
To do this we need to use rubys special command **#{}** inside this curly braces{} we can specify our variables.

```ruby
    var name = "Savitri"
    
    puts "Hello, my name is #{name} !!"
    
  // output: Hello, my name is Savitri !!
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

Comments are used when we want to add some information about the code which we dont want to be executed.
This helps the developer to remember why he has written the piece of code or it describes the functionality of the code.
There are two ways in which we can add comment to the ruby code 1) Single-Line Comment 2) Multi-Line Comment

### Single-line Comment
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
* It evaluates to true when one or the other or both expressions are true.

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

* This loop is used when you do know how many times you'll be looping.

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

1. my_arr = Array.new   // creates and empty array which looks like '[]'.
 
2. my_other_arr = []    // this is Literal Method to create empty array.

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
  key1 => value1, <br>
  key2 => value2, <br>
  key3 => value3 <br>
}
<hr>
### Creating Hashes

Using Literal form to create a hash. Here, my_hash is the name of the hash. 
It has 3 key-value pairs. The keys are "name", "age", "employee?" and "Savi", 22, true are its respective value.

```ruby
// liternal notation
my_hash = { "name" => "Savi",
  "age" => 22,
  "employee?" => true
}

puts my_hash["name"]
puts my_hash["age"]
puts my_hash["employee?"]

//output: Savi
          22
          true
```

You can create an empty hash with the new class method.
Here we are creating an empty hash named as "pets" and on the next line we are creating a key-value pair for it.
Here "tommy" is **key** and "dog" is **value**.

```ruby
// types to create hashes.
pets = Hash.new
pets["tommy"] = "dog"

puts pets["tommy"]

output: dog
```
<hr>

### Accessing Hash Values

Accessing the key-value pair from hash is same as accessing the items in an array.
For accessing the key-value pair from hash we are going to use **each** loop.

```ruby
// Accessing Hash Values:
family = { "Homer" => "dad",
  "Marge" => "mom",
  "Lisa" => "sister",
  "Maggie" => "sister",
  "Jane" => "grandpa",
  "Tom" => "dog"
}

family.each { |x, y| puts "#{x}: #{y}" }

// output:  Homer: dad
            Marge: mom
            Lisa: sister
            Maggie: sister
            Jane: grandpa
            Tom: dog

```

## Methods Or Functions

Methods Or Functions are body of code which we can reuse or call whenever needed.
The syntax says that we are defining a method called **welcome** and the **end** is declared when the method is complete.
We can define any complex functionality or output the statements etc.
The function or method can have single or multiple parameters. And we need to define this parameters when we are calling the function.

```ruby
Syntax:
def method_name
    //body .. //
end
```
In the first example we are defining a method called welcome, which simply outputs the message "Welcome to Ruby" when we call that method.

```ruby
Ex 1.
def welcome
    puts "Welcome to Ruby"
end

welcome // calling the method. 

output: Welcome to Ruby

```
In second example, we are defining say_name function which has one parameter name. Here name is a temporary variable which holds the value that we are going to pass when we call that function.

```ruby

Ex 2.

def say_name(name)
    puts "Hi, my name is #{name}. Nice to meet you!!"
end

say_name("Savitri")

//output: Hi, my name is Savitri. Nice to meet you!!
```

## Class

Classes in Ruby always is prefixed with the class keyword followed by the class name which start with a capital word.
It is a blueprint for some kind of object. 
In a class we can store variable, aslo we can define methods and access them.

```ruby 
syntax: class Welcome

        end
```        

In the example we are declaring a class called "Welcome", which has a method called hello.

```ruby
Example: 

class Welcome
    def hello
        puts "Hello World!!"
    end
end

var obj = Welcome.new   // creating an object.

obj.hello             //calling hello method of Welcome class.

//output: Hello World!!
```

# Ruby on Rails

Ruby on Rails is an extremely productive web application framework written in Ruby by David Heinemeier Hansson.
It is a web framework that makes it easy to build powerful web apps in a short amount of time.
Rails includes everything needed to create a database-driven web application, using the Model-View-Controller pattern.
Requires fewer lines of code than other frameworks.

## Setting up account on Cloud9.

For setting up your account on cloud9 click [here](https://ide.c9.io)

Visit the link mentioned above and create your account on Cloud9.
Cloud9 allows you to store your project work on cloud so that you can access it from anywhere, at any point till you have your internet connection.
It store your data for free. Also it has paid storage. For more information you can visit the site.

After successfully creating an account on Cloud9, follow the steps to create workspace for your project.

Step 1:  Click on the create a new workspace (+), you will be redirect to a new page where you will be fill up your project information.

Step 2: Enter your Project Name and Description. Select the "Hosted workspace" option as **Public**.

Step 3: Choose the template in which you want to use to build your project, here we will choose "Ruby on Rails".

Step 4: Create Workspace and you are good to go.

After successfully creating your workspace, you will be redirected to a window where you can see that a default rails application is already been created for you,which is been divided into 3 parts. 

* The **Left most** part shows a folder with the same name as you have given to your project. When you click on it, the folder unfolds to show bunch of another subfolders.
To learn more about the subfolders you can visit the [rails documentation section 3.2](http://guides.rubyonrails.org/getting_started.html#what-is-rails-questionmark).

* The **Right Upper part** of the window is where you are going to write your code.

* The **Right Lower part** of the window is the console, where you can test your code, check the version of ruby, write rails commands. 

## Rails Commands

In the console (**Right Lower part**), type the command 

**pwd**: This command tells you which directory you are currrently in.
     
```ruby

pwd
// output in the console: /home/ubuntu/workspace
```
     
**ls**: This command gives the folders and files in the directory.
     
```ruby

ls
//output in the console: Gemfile  Gemfile.lock  README.md  README.rdoc  Rakefile  app/  bin/  config/  config.ru  db/  lib/  log/  public/  test/  tmp/  vendor/
```
     
**cd filename**: This command is used to change the directory.
     
**ruby -v**: This command gives you the version of the ruby that is installed.
     
```ruby
ruby -v
//output in the console: ruby 2.3.0p0 (2015-12-25 revision 53290) [x86_64-linux].

``` 

**rails -v**: This command gives you the version of the rails that is installed.
     
```ruby
rails -v
//output in the console: Rails 4.2.5
```

```ruby
//To access rails console
Commamd: 
bundle exec rails console

Other Commands you can type in rails console. 

a.  Contact.new                               // used for creating Contact object
b.	@contact = Contact.new                   //storing the obj in variable @contact
c.	@contact.name = “name”                  //adding name/user name in db
d.	@contact.email = xyz@example.com       //dding email in db
e.	@contact.save                          //saving the data in db 
f.	Contact.first                         // to view the data at first position existing in db/table
g.	Contact.second                       //to view data at second position existing in the db/table
h.	Contact.all                         //to view all data in database.
i.	exit                               //to come out of console
j.	reload!                            //refresh the database if any changes made to it.

```

## Installing Rails

If you wish to install Rails on your PC you can visit [this](http://guides.railsgirls.com/install#setup-for-windows) website.

But here we will see the steps to install rails on Cloud9.

* We will start by creating an rails application and command to create the same is as follows:

```ruby
 rails new application_name

 example: rails new blog
```

This statement creates a rails application with the name **blog**.

* After creating the application we can navigate to that folder by:

```ruby
 cd blog
 
 bundle install
```

 This folder has auto-generated files and folders which will be useful further while developing the application. 
 
* After being in the application folder(blog), type "bundle install". This command will install all the gems required for the application which are located in the "Gemfile".
  If you get any error while running the "bundle install" try using "bundle update" command.


## To Start Rails Server

* To start the rails server you can use the command: 

```ruby
 rails server -p $PORT -b $IP or 

 rails s -p $PORT -b $IP
```

When you type this command in the rails console you will get a popup which will have the url link, where you can view your application.
Click on that popup box and you can see your application running.

Also you can go to the "Preview" at the top in the navbar and select "Preview Running Application".

* To Stop the server simply do Ctrl + C

```ruby
// to stop rails server.
 Ctrl + C
```

## Setting Git 

Any time you are setting git on your personal computer or for your application, follow the steps below:
You have to do this just once before starting up with any project work. You can know more about git by going to their wesite at [git-scm](https://git-scm.com/).
The **git** helps us to save our work as we progress with our application building process.
You can always track your work and if you ever make mistakes or screw up the with the code.

### Configuring git to your application

```ruby
cd project_name
git config --global user.name "Your Name"      // configuring our application with git.
git config --global user.email "your@email.com"
git config --global push.default matching   // as new versions of git come out it should still work the same for us.
git init                // initializing empty git reepository
git add .               // adding everything in this directory on git. ('.' means all)
git status              // it gives the names of the files newly added to the git.
git commit -m "Initial commit"     // saving all the files on git with the message.

```

### Steps to set an github account

Step 1: Go to [Github](https://github.com/) and create your **free** account.

Step 2: Go to https://c9.io/account/services, In the Github section click on "Connect".

Step 3: Type the console command: cat ~/.ssh/id_rsa.pub 
  **This command will print the SSH Key in the console output.**
  
Step 4: Copy the SSH Key generated in the console, go to https://github.com/settings/keys and on that page you need to fill up the "title" and paste the SSH keys in the "Keys" input box.
     Click on **Add Key** Button.
    
** NOW WE ARE SUCCESSFULLY CONNTED TO GITHUB **

<hr>

### Creating Repository on Github
     
Step 1: Login to your github account or if you are alreay logged in go to the home page.

Step 2: Click on the (+) sign on the top-right near your avatar.
        Click on new repository option from the dropdown list.
        
Step 3: You can start filling up the information. Give the name  for your repository, but for consistency name your repository same as your application_name.
        You can skip the description if you want to.
        You can choose a public repository if you want to share your code with other developers, or if you want to go for private you actually need to pay for an account.
        
Step 4: After clicking on "Create Repository" you will be redirect to a new page with Url as **https://github.com/User_name/application_name**.
        Click on the **SSH** button next to HTTPS.
        
        **Copy the command: git remote add origin git@github.com:yourusername/application_name.git**
        and paste it in the console. `(This command means that we are able to add out code to the particular address on github. )`
        
```ruby
git remote add origin git@github.com:yourusername/application_name.git

// output: you will not get any output. Next step explains you the verification.
```
        
Step 5: in console type "git remote".

```ruby
git remote

//output: origin
```

Step 6: in the console type command "git push origin master". This command will **push the copy of your application** on the github.
        Now if you go back to the page (https://github.com/User_name/application_name) mentioned in **Step 4** and refresh the page you can see the copy of your application on that page.

```ruby
git push origin master

```

```ruby
Syntax: git checkout -b branch_name   //to create new branch

Ex: git checkout –b site_pages        // creates a branch called ad site_pages in github directory.

Syntax: git checkout branch_name      // to change the branch 

Ex: git checkout development          // here we are changing out branch to development

Syntax: 
git checkout branch_name     // going to the branch with which we want to merge our branch
git merge branch_name        // combine two branches

Ex: git checkout master           // going on master branch
git merge layout_improvements     // combining layout_improvements branch with master branch

```

So now we have successfully sent a copy of our application on the github.

## Heroku setup

Heroku allows us to deploy our application to web. Which means that we are sending the copy of our application to another server where people can view our application.
It provides us with the **domain** or **web-address** where we can visit to see our application.

### Configuring Heroku on cloud9

Step 1: Go to Gemfile.

Step 2: Search a gem name 'sqlite3'.
        And modify it as `gem 'sqlite3', group: [:development, :test]`.
        
```ruby
    // Configuring Heroku on cloud9 Steps 2:
    `gem 'sqlite3', group: [:development, :test]`
```        

 This means that we are limiting out database gem sqlite to development and test environment.
 
Step 3: Underneath the sqlite gem defined in the gem file add this piece of code.

```ruby
Step 3: 
    // Configuring Heroku on cloud9 Steps 3:
In Gemfile: 

    # Use postgresql as the database for production
    group :production do
      gem 'pg'
      gem 'rails_12factor'
    end
```

```ruby 
 In console:
 
 bundle install --without production       //this command fetch the gem from the internet and installs it in our application.
 
 git status       // check the status of files that are modified.
 
 git add .       // add all the changes to git.
 
 git commit -m "Commit Message"     // commiting changes to the git.
 
 git push                    // sending the changes on the git.
 
```

### Setting up Heroku

Step 1: Create an account on heroku.com and Sing in into the account.

Step 2: In the console write 

```ruby
    // Setting up Heroku, Step 2.
    heroku login                     // this will prompt to login with the same credentials as that of heroku account.
```        
        Enter your email
        Enter your password          // the cursor would not move or nothing will appear when you are typing the password.

Step 3: In the console

``` ruby
 // Setting up Heroku, Step 3.
    heroku keys:add  // this will eastablish communication between cloud9 and heroku.
```

`This will ask you the confirmation whether you want to use the same public key. **Choose Yes(Y)**.`

Step 4: In the console

```ruby 
 // Setting up Heroku, Step 4.
 heroku create        // create a server in heroku
 
 // output : Git remote heroku added       // if everything is done correctly you get this output.
```

>While executing step 4 you will find a URL in the console. Save that URL somewhere because thats the URL for your application or the production or live application.

Step 5: In the console

```ruby 
 // Setting up Heroku, Step 5.
 git push heroku     // this will save the copy of your application on the heroku server.
 
```

Step 6: In the console 
You can repeat the following steps whenever you want to save a copy of your application to Github or Heroku.

```ruby
 // Setting up Heroku, Step 6.
    git status
    git add .
    git commit -m "commit message"
    git push 
    git push heroku 
    
```

```ruby
heroku domains             // it gives the url/link for your domain
```

## Scaffolding 

Rails gives us a special shortcut called **Scaffolding** by using which we can get a default rails generated skeleton structure of files.
This helps us to know about the rails file structure a bit and also how rails work.
The default structure created by rails for us by using the scaffold command are the Model, View, Controller, Database, Routes, Css files etc.
Here we don't have to individually create model files, views files, etc which saves a lot of time of ours to design the file structure, so we can say that scaffolding is shortcut to create our rails application skeleton.
You can go through the file structure that is created, also you can go through the list of files that are created by rails on the console when you execute the sacffol command.

One thing you need to do after successfully executing the scaffold command is that you need to do database migration. Basically what it does is perepares the database where we can store our data.
To know more about scaffolding you can visit [here](https://www.tutorialspoint.com/ruby-on-rails/rails-scaffolding.htm).

```ruby
Syntax: rails generate scaffold Application_name

Example: rails generate scaffold Post

//This command will create a model Post. It will also create accompanying views and a controller that contains the relevant CRUD actions and it also creates routes and database file. 

```

The **bundle exec rake db:migrate** command is going to look into the **migrate** folder and check the file and run them. Once the databaseis created successfully, you will get a confirmation in the console.

```ruby 
// execute this command after successfully executing scaffold command.

bundle exec rake db:migrate           
```

>It is recommended that after running the migration file, restart your serve.

## Controller

The controller is used to co-ordinate the function between user, model and view.
It receives the request from the application and matches with the particular route. 

The controller has class and class has different functions or methods which are called as **actions**.
Their are different actions like index, new, show, create, update, edit, delete and each action is associated with particular route. Also you can create your own methods.
Each action's responsibility is to collect information and provied it to the view.
Controller names starts with capital letter.

The class in the controller inherits the property of the parent controller **ApplicationController** which is loacted in controllers folder **application_controller.rb** file.
ApplicationController is again inherited from rails **ActionController::Base** class.

>Location of the controller file: You can find controller files in : /app/controller .

```ruby

rails generate controller controller_name

Example: rails generate controller Post.

//output: 

The controller file is created in the controllers folder.
 
class PostsController < ApplicationController
end

```

## View 

The view displays the information which a user of the website can see and interact with the website.

When we create the controller, it automatically creates a sub-folder under **app/views** with the same name as that of the corresponding controller's name. 
The files that we create in views has same name as that of the method_name that we define in the controller's class.

View templates are written in Embedded Ruby(eRuby) language. That is why ruby code is embedded inside the erb tags (<% ruby...code %>).
When you use <%= %> you render the expression value to your output. 
While <% %> is to write some Ruby code that won't be rendered to final output.
Also the view files has the extension of **.erb** .
The data between view and controller is shared through mutually accessible variables.

```ruby
//Example of View File

<p id="notice"><%= notice %></p>

<h1>Listing Recipes</h1>

<table>
  <thead>
    <tr>
      <th colspan="3"></th>
    </tr>
  </thead>

  <tbody>
    <% @recipes.each do |recipe| %>
      <tr>
        <td><%= link_to 'Show', recipe %></td>
        <td><%= link_to 'Edit', edit_recipe_path(recipe) %></td>
        <td><%= link_to 'Destroy', recipe, method: :delete, data: { confirm: 'Are you sure?' } %></td>
      </tr>
    <% end %>
  </tbody>
</table>

<br>

<%= link_to 'New Recipe', new_recipe_path %>

```

>Location : You can find the views in /app/views .

To know more about ERB you can refer [this](https://docs.puppet.com/puppet/latest/reference/lang_template_erb.html) page.
To know more about view you can refer [Rails Guides](http://guides.rubyonrails.org/layouts_and_rendering.html).

## Routes

The routes are loacted in the **config/routes.rb**.
When you go the routes file loacated at the above position you can find the commented code in it.
That code is nothing but the examples of routes provided by rails to you, so that you can understand how to create your own routes.

The special keyword used to create routes for our application is **resources**.
Instead of declaring separate routes for your index, show, new, edit, create, update and destroy actions,we can do it in a single line by using resources keyword.
The resources tells rails that you want to create routes that matches particular controller's actions.

You can also view the routes or url associated with the specific controller action in the console by using the command **bundle exec rake routes**.

For more information about routes you can visit [Rails Guides](http://guides.rubyonrails.org/routing.html).

```ruby
// to define routes.

Syntax :
resources :controller_name

Example
resources :recipes

resources :books
```

##Active Records

Active Records are the Model from the MVC.
The Model is used to manage the data and store the data in the database.
Each Model object has CRUD (Create, Read, Update, and Delete) methods for database access.

The Model files names are **singular** with first letter **capital**, whereas the assciated Database table name is **plural** and written in **CamelCase**.
The model files are inherited from **ActiveRecord::Base** class.

Since the data we enter into databse is defined in rails Model we put the **validation** to our data in the Model files. Validations are used so that we can store correct data in our database.
For example we want to store correct email address or we want all fields of the for to be filled properly.
To know more about validation visit [here](http://doc.bccnsoft.com/docs/rails-guides-3.2-en/active_record_validations_callbacks.html).

```ruby
//  Validation Example:

class Employee < ActiveRecord::Base
  validates :name, :presence => true
end
 
Employee.create(:name => "Savitri M").valid? # => true
Employee.create(:name => nil).valid? # => false
```

Example:

Model     | Table
----------|-------
Book      |	books
OrderItem | order_items
Person    |	people

```ruby
Syntax: rails generate model Modelname

Example: rails generate model Book
```

**Database:** Databases are like the hard-drive of the web. We store information to the database permanently and then we access this information later whenever we want.
For example we create an account on facebook, post pictures, comment on pictures do lot of stuff. This all information is stored in the facebook's database which we are able to access the next day we login to our facebook account.
Database are like spreadsheets with rows and columns.

**Migration:**  A migration is a way to update the database with a new table, or changes to an existing table.
When we create a Model using rails generator, an associated migration file is also create in the **db** folder with the timestamp.
This migration file is nothing but the database table in which we can define multiple columns with their datatypes.
By default rails creates a **primary-key** column in every database table with datatype as **integer**.

Basic datatypes supported by migration file are:

* string − is used when we want to store data as small data types such as a name.

* text − is used when we want to store data as longer pieces of textual data, such as the description.

* integer − is used when we want to store data as whole numbers.

* float − is used when we want to store data as decimals.

* datetime and timestamp − store the date and time into a column.

* date and time − store either the date only or time only.

* binary −is used when we want to store data such as images, audio, or movies.

* Boolean − is used when we want to store data as true or false values.
 
>Location of model file is app/models folder.

## Association 

In our application we have multiple Models and we would also like to have some connection between those models, so to do that rails provides us with **Association**.
Association in rails is used to connect tow or more Models.

Types Of Association:

* belongs_to
* has_one
* has_many
* has_many :through
* has_one :through
* has_and_belongs_to_many 

To know more about "Association" visit [here](http://doc.bccnsoft.com/docs/rails-guides-3.2-en/association_basics.html).

## REST (Represenatational State Transfer)

REST says that `Refer to "thing" on a web as "resource"` AND  `you should be able to 1) Create 2)Read 3)Update 4) Delete (CRUD)this resources`.
The resource can be a facebook profile or linkedIn Profile or a picture on Instagram etc.

CRUD example, suppose you want to create an account on facebook you first create an user-profile when we login for the first time, so this represent your **CREATE** action.
Then you are able to view your profile that you have created, this represent your **READ** action. If you wish to make some changes in your profile you can edit your profile, this represent **UPDATE** action.
And if you wish to delete your profile you can delete it, this represent to the **DELETE** action.

Most of the modern webs follows this concept of REST, where you can Create, Read, Update, Delete resources on web.

### HTTP Request

GET: This is most commom type of http request.  
Whenever you want to open a particular page or website like facebook.com or youtube.com you are sending a HTTP Request that has GET method.

POST: Whenever you are submitting a form you are sending a HTTP Request that has POST method.
For example whenever you are submitting the Facebook's user-profile form you are sending POST request to their server.

PUT/ PATCH: Whenever you are updating data on the web you are sending PUT/ PATCH request to the server.
PUT	is used to completely update a resource. For example, updating your user profile on facebook or linkedIn etc.
PATCH is used to partially update a resource. For example, when we are just updating the password for your user profile.

DELETE: Whenever you want to delete data from web you will find that the request method is DELETE.

###Processing HTTP Request

1. Browser send HTTp request to the web-server.
2. The web-server catch that request and sends it to the Routes file in the rails application.
3. The routes file communicates with the controller
4. The controller then gathers the data from **Model file** and Template from **View file** and sends it back to the web-serverwhich then packages everything as HTTP Response.

## User management

Rails uses special gem called "devise" for managing the user. This includes 
You can visit the [github documentation](https://github.com/plataformatec/devise) to follow the steps about the installation of the devise gem.
For checking the latest version of the devise gem visit [here](https://rubygems.org/gems/devise/versions/3.5.6).

# Javascript

Html is used to add content on the web-page, CSS allows us to add some colour or postion things on the page.
It helps to make Html look attractive, but what about interaction ? So here Javascript comes into picture.
Javascript is a programming language which is been used for making the website interactive.
Making page interactive means we can click on the button and some action happens or when we hover over a link it colour changes or it enhances etc.

**Types to include javascript in your HTML** 

* **External**
You can create a separate javascript file with ".js" extension and save it in the folder along with the other files of the application.
Once you have save saved the file successfully, you can give the link to that file by specifying the path under **head** tag, in **script** tag.

```javascript

    <DOCTYPE html>
    <html>
      <head>
        <title>Javascript Test</title>
        //here demo.js is your external javascript file.
        <script src="demo.js"></script>  
      </head>
      
      <body>
            <h1>Hello</h1>
      </body>
    </html>  

```

* **Internal**
In this type you can directly include javascript code in the HTML code under **head** tags.

```javascript
      <DOCTYPE html>
    <html>
      <head>
        <title>Javascript Test</title>
        //internal javascript.
        <script>
            alert("Hello from inside of the HTML");
            prompt("What is ypur Name?")
        </script>  
      </head>
      
      <body>
            <h1>Welcome</h1>
      </body>
    </html> 
```

## Variable 

They allows us to label a piece of code so that we can reuse it later.
Always declare the code in either <script></script> tags or in the javascript file.
A variable can hold string, numbers, arrays etc. values.
In the example we declare the variable in side the script tag.

```javascript
     <DOCTYPE html>
    <html>
      <head>
        <title>Javascript Test</title>
        <script>
         var name = "Savi"; 
            alert(name);  // This prints the Value stored in the name variable in the alert box.
        </script>  
      </head>
      
      <body>
            <h1>Welcome</h1>
      </body>
    </html>
```

## Scope

Scope is set of variables, object, functions, methods etc which we can access and use to store data.

Local scope of variable means that the variable can be accessed only within a function or method where it has been defined.
local scope of a variable is set when a function is initialized and is destoryed when the functionis executed. 

Global scope of variable means that the variable can be accessed anywhere within the function by other methods.
It is set when we start the program and is destroyed when the program is stopped.
Variables with global scope are initialized outside the function.
We can define global scope variable and local scope variable with the same name.

Checkout the examples to understand more about the scope and how they work.

```script

A globally-scoped variable
var a = 1;

// global scope
function one() {
  console.log (a); // output in console: 1
}

// Local scope
var a = 1;

function two(a) {
  console.log (a); // output the given argument, not the global value of 1
}

```

## String

Strings are declared inside the quotation marks (" " ,' '), else you will get an error.
There are few operations that you can do on strings,you can do string **concatenation**, means you can add two or more strings to form a large string.

```javascript

// you can run this command in the broswers console.
 "My name is" + " Savitri M."
 // output: "my name is Savitri M"

```

**Length of string**

To find the length of a string you can use **.length** method.

```javascript
var name = "Savitri";

console.log(name.length);

//output: 7 (displayed in the browser console.)

```

**Substring** 

Substring method is used to divide the string into parts.

```javascript

var name = " My name is Savitri";

console.log(name.substring(0,11 ));
//output:  My name is
```

## Maths

You can perform few mathematical operations like addition, substraction, multiple, divide, etc. in the browser console to practise and if you want you can use it in your application.
You can perform mathematical operations on numbers only. 
If you try to add number and string it will do the string concatenation operation.

```javascript

Example of Maths 

87*69
 // output: 6003
3.2+2.66
 // output: 5.86
55/10
 // output: 5.5
20%4
 // output:0
20+60-40*5
// output: -120

Maths on numbers and string:

"hello"+5
 // output: "hello5"
"hello"/5
 // output: NaN
"hello"*5
 // output: NaN
 
Using variable: 

num1 =50 
// output: 50

num2 = 60
// output: 60

num1*num2
// output: 3000
 
num3 = num1+num2
// output: 110

```

## Boolean 

Boolean value returns true or false as an output. Based on the value of the booleans you can use conditions in your code or manipulate some code etc.

```javascript
2>3
// output: false

5!=5
// output: false

3==3
// output: true

2 == "2"
// output: true

```

## Control Flow 

**If-else Statement**

Control Flow includes "If-else" statement.
It means that depending upon the condition either one piece of code will execute or the other piece of code will execute.

```javascript

Syntax:

if(condition){
    // some code
}
else
{
    //some other code
}

Example: 

if(2 < 5)
{
    alert("2 is less than 5");
}
else
{
    alert("False");
}

```

<hr>

**Switch Statement**

Another type of control flow statement is **switch** statement.
You can use switch statement if you are annoyed by typing if-else statement for more number of times. At that time you can use switch statement.
The switch statement provides you to present multiple option called the cases then check an expression to see if it matches any of them. 
If there's a match, the program will perform the action for the matching case, if there's no match, it can execute a default option.
Have a look at example to know about the switch case.

```javascript
// code for switch case

var subject = prompt("Which is your favorite subject ?","Type your subject choice here");

switch(subject){
  case 'java':
    console.log("Sure thing! you have to learn OOPS!!");
    break;
  case 'HTML':
    console.log("Got it! You want to build a website.");
    break;
  case 'AngularJs':
    console.log("Sounds good! Its a new technonlogy. Go with it");
    break;
 
  default:
    console.log(" Everyone has their own choice !! Yours is " + subject );
}

```


## Comments

To use comments you need to put two forward slashes (//) in front of any statement that you need to comment out.
To do multiple line comment you need to use /* ... */ symbols.
Comments are simply used to add some side notes when we are writing the code. 
It helps you to remember why you have written a piece of code, so that even if you come back after a long time you would be able to continue with the same flow.

```javascript
// hello, this is a commented statement

/* this
 is 
 multi-line
 comment.
 */ 

```

## Loops

Loops in javascript are kind of iterators, they allows us to write a piece of code and repeate the code number of times we want to depending upon some condition.
Their are two types of loops 1) For loop 2) While loop.

**While loop**

While loop executes the piece of code till the while condition is sets to false.

```javascript
Syntax 

while(condition){
    // code //
}

Example

var i = 1;

while(i<5)
{
    console.log(i);
    i = i + 1;
}

//output: 
1
2
3
4
5
```

**For loop**

The for loop also executes a piece of code till the time a condition is satisfied.
In for loop we write 3 statements, 1) In the first statement we declare a variable and initialize it 2) In second statement we put our condition 3) In third statement we increment/decrement the variable.

```javascript

for(var i = 0; i<5; i++){
    console.log(i);
}

//output :
0
1
2
3
4

```

## Array

Arrays are used to store a collection of data. 
In an array you can save the data of the same type or different types.
Arrays are fixed length datatype. The elements stored in the array possess property of index. 
Index are nothing but numbers or the positions that each elements in an array possess.
We can access the elements in an array with the help of this index.
Array index starts from '0', which means that the first element in an array will have index zero.
It lets you store multiple values together such as numbers, strings, arrays, etc.

Types to declare Array

1) var x = new Array

2) []  // creates an empty array

To insert an element in an array we use .push method. The push method insert an element at the last position of an array or at the end of an array, ypu can check the example below.
To remove an element in an array we use .pop method. The pop method removes the elemet at the very last position and returns it.

```javascript

var x = new Array

//output: []

x.push("string",5,33)

//output: ["string",5,33]

x[0] ;    // accessing the element by specifying their index

// output: "string"

x.pop()                 // to remove an element from an array
//output: 33         //returns an item that is removed from an array.

console.log(x);
//output: ["string",5]

x.push("Hello")
// output: ["string",5,"Hello"]
```

```javascript
 // To iterate over an array
 
 var subjects = ["HTML","JavaScript", "Ruby"];
for(var i = 0; i < subjects.length; i++)
{
 console.log(subjects[i]);   
}

//output: 

HTML
JavaScript
Ruby

```

## Functions

Functions in javascript helps us to reuse a block of code, so that we dont have to keep rewriting things in multiple parts of our program.
We write function name in camelCase. To declare a function we use a special keyword **function**.

```javascript

// declaring the add function with two parameters.
var add = function(a,b)
{
    console.log(a + b);
}
 
add(5,6)  // calling the add function by passing the parameters.

//output: 11

```

## Object

Objects are another datatypes in javascript. They allow us to organize our code.
Object has properties and methods.
They store the data in the form of key-value pair,the key can be number, string or variable.

Ways to define an object:

1) var myself = {}              // creates an empty object.

2) var myself = new Object();     //

```javascript

// literal notation to create an object
var myself = {
    
    name: "Savi",
    place: "Mumbai",
    phone: "222-222-222",
    age: 20
}

// constructor notation
var myself = new Object();
myself.name = "Savi";
myself.place = "Mumbai";
myself.phone = "222-222-222";
myself.age = 20;

//output : Object {name: "Savi", place: "Mumbai", phone: "222-222-222", age: 20}
```

```javascript

You can add functions as property of an object externally
myself.say = function(){ console.log("You are the worst!!")}

myself.say          
// output: { console.log("You are the worst!!")}

myself.say()
// output: "You are the worst!!"

Accessing Data From Objects:

myself.name           // accessing the name property
//output: "Savi"

myself.phone          // accessing the phone property
//output: "222-222-222"

Alternate methods to access the data from object:

myself["phone"]
//output: "222-222-222"

myself["age"]
//output: 20

```

### Creating an object with user defined function

First of all we define a constructor by passing it the desired number of parameter and then use that function to create our objects.
The constructor uses this keyword to set the dynamic properties that we pass to a constructor function.

```javascript
// creating a constructor
function Person(name,age) {
  this.name = name;  //this.name is a placeholder that holds the value of name property
  this.age = age;
 }
 
 // creating object using that constructor.
sav = new Person("Savitri", 20);   
// output: Person {name: "Savitri", age: 20}

bob = new Person("BOB", 25);
// output: Person {name: "BOB", age: 25}

bob.name      //accessing the name property of bob object
// output: "BOB"

sav.name      //accessing the name property of sav object
// output: "Savitri"

```

```script

Accessing an html element

 <DOCTYPE html>
    <html>
      <head>
        <title>Javascript Test</title>
        //here demo.js is your external javascript file.
        <script src="demo.js"></script>  
      </head>
      
      <body>
            <h1 id="h1">Welcome</h1>
            
            <p class="para" >This is a paragraph.</p>
            <p class="para" >This is another paragraph.</p>
            
            <script>
                var h = document.getElementById("h1");
                output: <h1 id="h1">Welcome</h1>         
                
                var p = document.getElementsByClassName("para");
                output:  returns an array 
                [<p class="para" >This is a paragraph.</p>, <p class="para" >This is another paragraph.</p>]            
                
                var t = document.getElementsByTagName("para");
                output:    returns an array 
                [<p class="para" >This is a paragraph.</p>, <p class="para" >This is another paragraph.</p>]       
                        
                querySelector allows us to grab things using the CSS.                
                var q = document.querySelector("h1")
                output: <h1 id="h1">Welcome</h1>            
                
                // Accessing all the h1 tags using CSS
                var q1 = document.querySelectorAll("#h1")
                output: <h1 id="h1">Welcome</h1>            
            
            </script>
      </body>
    </html>

```

## Javascript Events

Javascript has the concepts of events that allows us to track all kinds of events, eg mouseclick, scroll, keypress etc.
Using javascript we can put event_handlers on the HTML elements so that when an event occours it can show some action kind of thing.
You can find different types of event handlers [here](http://www.w3schools.com/jsref/dom_obj_event.asp). which you can use in your website.
You can refer above examples to see how we cantarget the HTML elements.


**Event listner:**

Event listener is a function that takes two parameter, the first parameter is the event_name such as click, drag, scroll etc. and the second parameter is the action that we want to happen when the event occours.

```script
//Example of adding event listner

<script>
  
      var func = function myFunction() {
       alert ("Hello World!")
      }

      document.addEventListener("click", func);
      
</script>

//output: here when you click anywhere in the broswer you will get an alert box displaying the message Hello World! .

```

# jQuery

jQuery also allows us to add interactive code to our website or to HTML content.
The Html document is designed and structured according to the [DOM](http://www.w3schools.com/js/js_htmldom.asp).
With the help of DOM we can access and modify the HTML.
To use jQuery in your application you need to include it in your Html file and the way you can do that is by searching on web for [jQuery CDN](https://code.jquery.com/).
Now from there you can pickup any version of jQuery and include in your Html document, so that you can link your application with jQuery.

To refer a jQuery documentation you can always visit [this site](http://api.jquery.com/). 

## jQuery Syntax

Syntax: $(selector).action()

Syntax Explanation:  jQuery uses special symbol **"$"** to **access** jQuery, the **selector** is **find the specified html element** and the **action** is **operation to be performed on the targeted element**.

jQuery uses CSS to access the elements and after targeting the specific element we can put some styles on it or we can ask it do some actions, so as to make the website interactive.
You can find the numbers of styles that you can use [here](http://www.w3schools.com/jsref/dom_obj_style.asp).

```script
 $("#notready").fadeOut(1000);
 
// here we are selecting the element by targeting the id="notready" which must be defined in your HTML and then adding the action of fadeOut after 1000ms.
```

We write jQuery code in a special block **"$(document).ready(function(){ ... jQuery code ... });"**. 

Explanation: 

The **$** sign represent that it is a jQuery code.
**(document)** tells that we are about to work on HTML document.
**.ready()** tells that it will run  the function when HTML document is ready. And whatever inside the ready block will execute when Html document is ready.

```script
<!DOCTYPE html>
<html>
<head>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
<script>
$(document).ready(function(){
    $("button").click(function(){
        $("p").fadeOut(2000).fadeIn(5000);
    });
});
</script>
</head>
<body>

<h1>Welcome to jQuery</h1>

<p>This is a paragraph.</p>
<p>This is another paragraph.</p>

<button>Click me to see paragraphs fading Out and then fading In!!!</button>

</body>
</html>

```

# AngularJs 

AngularJs is a web development framework based on Javascript and is open source means it is freely available to its users.
Many developer use AngularJs to make dynamic web application. AngularJs is currrently maintained by "Google".
It is categorized as MV* framework. M is model where you can store your data. V is view where user is used to view data on your web-page.
'*' can be Controller or ViewModel  or can be something else. AngularJs uses Controllers and hence we call it is as MVC based framework.

## Features

* Data Binding: Means that when the data in the model changes it reflects in the view and when the data in the view changes it is reflected in the model.
             This means that data-binding is synchronization between model and view.
 
* Dependency Injection:  It helps you to encapuslate a piece of your application code and use it later whenever needed and it also improves testability.

* Controller: Everything in angular starts with the **Controller**. In Controller we write the logic. Controller are the function that are bound to **scope**.

* View: View contains bindings and directives. Controller can communicate with View by using one-way or two-way binding.

* Services: Services are also kind of functions, which holds complex logic of our application.

* Directives: AngularJs has the ability to extend the Html by the use of `directives`. They are prefixed with **ng-**.
              They can be used to make custom Html tags.

* Filters: Filters are used to Format, Sort and Filter Data. It is used with the binding expression or directives.

* Scope: This are the objects that refer to the model. They allow controller and view to communicate with each other.

## Expression 

Expression in AngularJs are used to bind data to the Html.
They are always denoted by "{{ }}" two curly braces.
We can write operators, numbers, variable etc in the expressions.
Expressions can also be written inside a directive: ng-bind="expression"

In the example different types of expessions are been given along with its output.
You can find the description of directive in its section.

```script

// Example of Expression

<!DOCTYPE html>
<html>
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.4.8/angular.min.js"></script>
<body>

<div ng-app ng-init="f_name = 'Savitri'; l_name = 'Mhatre'">

<p>{{ "Hello"}} </p>
<p>{{ 5 + 5 }}</p>
<p>This is me: <span ng-bind="f_name+ ' ' +  l_name" ></span></p>
</div>

</body>
</html>

// output: 
Hello

10

This is me: Savitri Mhatre

```

## Modules 

An AngularJS module defines an application.
It is a container for every piece of angular application. The modules in the Angularjs is created by using "angular.modules".
It takes two inputs, the first is the name of the application. This name is same as that which we define in the "ng-app" in out Html document.
The second parameter is the list of other modules that this module is dependent on. If there is no other dependent module then simply declare an empty array "[]".

The [] parameter in the module is used to define dependent modules.

After declaring a module you can further define controller, directive, services etc to your angular application.


## Directive

Angular has build-in directives that are used to add functionality to your application..

* ng-app : It is used to tell Angular Html page is an AngularJs application.
The ng-app is called a directive.
It tells AngularJS that the myApp module will live within the <html> element.
We used the ng-app directive to define the application scope.

```script
// Example of directive and module

<html ng-app="myApp">...</html>                 // directive.

<script>

var app = angular.module("myApp", []);       // module.

</script>

```

* ng-init: This directive is used to initialize the application data.
 It is used to assign values to the variables. In the following example, we initialize an array of countries.

```script

//Example of ng-init

<div ng-app="" ng-init="countries=['India','United States','United Kingdom','France']">
...
```
* ng-model: The ng-model directive defines the model/variable to be used in AngularJSmApplication. 
In the following example, we define a model named name.

```script

//Example of ng-model

<div ng-app="">
...
<p>Enter your Name: <input type="text" ng-model="name"></p>
</div>

```

* ng-repeat: ng-repeat directive repeats the Html for each item in a collection.

```script
// Example of ng-repeat

<div ng-app="">
...
 <p>List of Countries:</p>
 <ol>
 <li ng-repeat="country in countries">
 {{ 'Country: ' + country }}
 </li>
 </ol>
</div>

//output: 
List of Countries:
1. Country: India
2. Country: United States
3. Country: United Kingdom
4. Country: France

```

* ng-show: It is used to show a given control.
 
```script
// Example of ng-show directive

<input type="checkbox" ng-model="showHide1">Show Button
<button ng-show="showHide1">Click Me!</button>

```

* ng-hide: It is used to hide a given control.
 
```script
// Example of ng-hide directive

<input type="checkbox" ng-model="hide1">Hide Button
<button ng-hide="hide1">Click Me!</button>

```

* ng-click: It is used to add click event in the angular application.

```script
<p>Total click: {{ clickCounter }}</p></td>
<button ng-click="clickCounter = clickCounter + 1">Click Me!</button>
 
```

## Controller 

Controller control the data of AngularJs application.
It is defined as "ng-controller". It is also a kind of directive.
It has a "$scope" object.
Using the $scope object we can create the properties on the Controller and then can access it later by using ng-model or using expressions.
We can also define the controller object in a separate JS file and refer that file in the HTML page.

```script
<!DOCTYPE html>
<html>
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.4.8/angular.min.js"></script>
<body>

<div ng-app="myApp" ng-controller="personCtrl">

// accessing the properties using ng-model

First Name: <input type="text" ng-model="firstName"><br>
Last Name: <input type="text" ng-model="lastName"><br>
<br>
Full Name: {{fullName()}}

</div>

<script>
var app = angular.module('myApp', []);
app.controller('personCtrl', function($scope) {

// declaring the properties using "$scope" object.

    $scope.firstName = "Savitri";
    $scope.lastName = "Mhatre";
    $scope.fullName = function() {
        return $scope.firstName + " " + $scope.lastName;
    };
});
</script>

</body>
</html>

//output:
First Name: Savitri

Last Name: Mhatre


Full Name: Savitri Mhatre

```

## Filters

Filters are used to modify data. We can club them in expression or directives using pipe(|) character.

Types of filters:

* uppercase: It converts text to uppercase text.

```script
// Uppercase Example:

Enter first name:<input type="text" ng-model="person.firstName">
Enter last name: <input type="text" ng-model="person.lastName">
Name in Upper Case: {{person.fullName() | uppercase}}

```

* lowercase: It converts text to lowercase text.
 
```script
// Lowercase Example:

Enter first name:<input type="text" ng-model="person.firstName">
Enter last name: <input type="text" ng-model="person.lastName">
Name in Lower Case: {{person.fullName() | lowercase}} 

```

* currency: It formats the text into the currency format.

```script
// Currency filter Example:

Enter fees: <input type="text" ng-model="cart.cost">
fees: {{cart.cost | currency}}
 
```

* filter: It returns the subset of an array based on the given condition.

```script

// Example of the Filter

Enter subject: <input type="text" ng-model="subjectName">
Subject:
<ul>
 <li ng-repeat="subject in student.subjects | filter: subjectName">
 {{ subject.name + ', marks:' + subject.marks }}
 </li>
</ul>

```

* orderby: It is used to order the array based on the given condition.
 
```script

// Orderby Filter Example:

Customers:
<ul>
 <li ng-repeat="customer in customer.customers | orderBy:'age'">
 {{ customer.name + ', Age:' + customer.age }}
 </li>
</ul>


```

## View

AngularJs supports single page application via multiple views on a single page. It means we can link multiple page on the single page.
To do this angular provides ng-view directive and $routeProvider service.

* ng-view directive

ng-view directive acts as a placeholder where a corresponding ng-template/view can be placed.

```script
// Example of ng-view

<div ng-app="myApp">
    ...
 <div ng-view></div>
</div>

```

* $routeProvider Service

If you want to navigate to different pages in your application without reloading the page you can use the ngRoute module.
The $routeProvider is used to set the configuration of URLs, maps them with the corresponding HTML page, and attaches a controller with the same.
To use the routeProvider service we need the "ngRoute" module to be installed.

```script

app.config(function($routeProvider) {
  $routeProvider
  .when("/", {
    templateUrl : "main.htm"
  })
  .when("/home", {
    templateUrl : "red.htm"
  })
   .when("/about", {
    templateUrl : "red.htm"
  })
  
});

```


## Scope

Scope provides binding between view and controller.
To access the data we use $scope object.
$scope is used to create variables and functions in the controller.

```script

<div ng-app="myApp" ng-controller="myCtrl">

<h1>{{petname}}</h1>

</div>

<script>
var app = angular.module('myApp', []);

app.controller('myCtrl', function($scope) {
    $scope.petname = "Tito";
});
</script>

```

## Services
To perform specific function or task we use services.
By the means of services we can keep our logic separate from the main code to avoid complexity.
Also we can use the same piece of code multiple times whenever needed so as to avoid repeatation.
We can use a particular service by simply using the concept of dependency injection.
Angular has provided us with default services such as $http, $route, $window, $location etc and also provided the ability to create new services.
The inbuilt services are always prefixed with "$" symbol.

There are two ways to create a service by using the keywords as follows.

1) Factory:

In this method, we first define a factory and then assign method to it.
Factory is a function which is used to return value.

```script

// to declare a service using "factory" keyword:

var myApp = angular.module("myApp", []);
 myApp.factory('Maths', function() {
 var factory = {};
 factory.multiply = function(a, b) {
 return a * b
 }
 return factory;
 });

```

2) Service:

In this method, we define a service and then assign method to it. We can also inject an already available service into this.
Service is defined using service() function and it is then injected into the respective controller as needed.

```script

myApp.service('CalcService', function(Maths){
this.square = function(a) {
return Maths.multiply(a,a);
}
});

// injecting the service in the controller.
myApp.controller('CalcController', function($scope, CalcService) {
$scope.square = function() {
$scope.result = CalcService.square($scope.number);
}
});

// to take input and display output.

<div ng-app="myApp" ng-controller="CalcController">
<p>Enter a number: <input type="number" ng-model="number" />
<button ng-click="square()"></button>
<p>Result: {{result}}</p>
</div>


//Example:
Enter the number: 5

Result: 25
```

# Firebase 

##Introduction

Firebase provides us the facility to store and manage our data with its “No SQL” cloud database.
Data is synced across all clients in realtime and data also remains available if the app goes offline.
The data stored in the firebase is in the JSON format.

## Setup
To use Firebase as your database you need to do the following setup:
1.	Create a Firebase project by going to the [firebase console](https://console.firebase.google.com/) if you don’t have a project.
Click n Create New Project to create a new project.
You can also import your project by clicking on Import Google Project.

2.	Once you are done with Step 1, click on the project. Once you are redirected to the new page click on “Add Firebase to your web app”.

3.	A pop with will appear which contains some code snippet. Copy that snippet and add it into your project.
This snippet contains initialization information to configure firebase into your project.

## Authentication

###Anonymous Authentication: 

Anonymous authentication is been done when the user wants to login only for a single session. The user does not have to enter any credentials to login as anonymous.
Anonymous Login setup:

You need to follow the steps below
a)	In the Firebase console open the Auth section.
b)	On the Sign-in Methods page, enable the Anonymous sign-in method.
c)	Call the firebase signInAnonymously() function in your controller file.

```firebase

Firebase.auth().signInAnonymously().then(function(){
//Successful
}).catch(function(error){
// Handel Error
});

```
<hr>

### Password Authentication 

We use this type of authentication method when the user needs to login to the account
You need to follow the steps below:
a)	In the Firebase console open the Auth section.
b)	On the Sign-in Methods page, enable the Email/password sign-in method.
c) Add the below code to your controllerfile.

The `createUserWithEmailAndPassword()` method is used when we want to create a new user or when the user logins for the first time.

The `signInWithEmailAndPassword()` method is used so the user can login with the same credentials as he used when he logged in for the first time. 

The `signOut()` method is used so that user can successfully signout.

```firebase

firebase.auth().signInWithEmailAndPassword(email, pass).then(function(){
console.log('Signed In Success')
});
promise.catch(e => console.log(e.message));

});


firebase.auth().createUserWithEmailAndPassword(email, pass);
promise.catch(e => console.log(e.message));

});


firebase.auth().signOut().then(function() {
  // Sign-out successful.
}, function(error) {
  // An error happened.
});

```
<hr>

### SignIn with Facebook

Using this method the user can use his facebook account credentials to login to an application.

Follow the [video]( https://www.youtube.com/watch?v=8XnUs2xY5c4&feature=youtu.be) do the setup setp by step.

```firebase

auth.$signInWithPopup("facebook").then(function() {
// successful signin
}).catch((function(err) {
// An error happened.
})
```

## Read Write Data:

To read and write data to the database you need a instance of firebase.database.Reference.
A Reference represents a specific location in your database and can be used for reading or writing data to that database.

```firebase

// Get a reference to the database service
var database = firebase.database().ref();

or

var database = firebase.database().ref("child/path");

```

* Write:

Write means we are writing or storing the data to the firebase database.
In firebase we need to provide the reference where we want to store the data.
For write operations, you can use "$add()" to save data to a specified reference.

```firebase

// Inside  Controller named as CategoriesCtrl
function() {
      firebase.database().ref().child("/categories/").$add({name: this.newCategoryName});
}
```

In the example we are storing the data to the child reference named as "categories" which has the property as "name".
You can add as many properties to this child node.

* Read:

For the read operation you again need the reference of the child node from which you want to retrive or read the data that is available in the firebase database.
Here we are using the firebase's "$firebaseArray() service" to retrive the data from the firebase database.
This service takes a Firebase reference and returns a JavaScript array which contains the data at the provided Firebase reference.

```firebase

// in controller file

var ref = firebase.database().ref().child("/categories/");

$scope.categories = $firebaseArray(ref);


// in view file

<div class="row" ng-controller="CategoriesCtrl">

<tr ng-repeat="category in categories">
  <td>{{category.name}}</td>
</tr>
</div>
```

In the ng-repeat loop the "categories" is defined in the controller file and we are linking the controller file and view file by using "ng-controller".


* Delete

To remove a data from the firebase database we use firebase's "$remove()" method.
This method returns a promise that will be fulfilled when the data has been removed from the server. 

In the example  $scope.removeCategory is the name of the function which we we will call when we want to remove a particular data.

```firebase

//in view file

<tr ng-repeat="category in categories">
  <td>{{category.name}}</td>
  <td><a class= btn btn-danger" ng-click="removeCategory(category)">Delete</a>
</tr>

// in controller file

$scope.removeCategory = function(contact){
    $scope.contacts.$remove(contact);
}

```

* Update

This are the steps to update the stored data in the database.

```firebase

//in view file

<tr ng-repeat="category in categories">
  <td>{{category.name}}</td>
  
  // to select the category that we want to edit.
  <td><a class= btn btn-primary" ng-click="EditCategory(category)">Edit</a> 
  
  <td>
  //to update the edited category.
    <button type="button" class="btn btn-primary" ng-click="$ctrl.updateCategory()">Update</button>
    
 // to cancel if you dont want to perform edit.    
    <button type="button" class="btn btn-warning " ng-click="$ctrl.cancelEdit()">Cancel</button>
  </td>

</tr>

// in the controller file

//  this function is used to select the data that we want to edit.

$scope.EditCategory = function(category){
    $scope.id = category.$id;
    $scope.name = category.name;
}

// to save the data after we are done with the editing

$scope.updateCategory = function(){
	var id = $scope.id;
			
// Returns the record from the array for the given key, If key isn't found it returns null. 
	var record = $scope.events.$getRecord(id);
	console.log(record);
	record.e_name = $scope.e_name;
			
	$scope.categories.$save(record).then(function(){
	    	console.log('updated category');
	}		
}

// Cancel the Edit

$scope.cancelEdit = function(){
    // return to the home page.
}
```