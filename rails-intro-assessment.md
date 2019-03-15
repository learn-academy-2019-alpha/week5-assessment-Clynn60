Carrie Johnson
# Week 5 Assessment

Try your best to answer each question on your own before looking up the answer online. Once you're done writing your first answer, you can google the question and write the best answer you find.

### 1. What are some advantages of using Ruby on Rails?
-Less syntax, more user friendly

### 2. How does Ruby on Rails use the Model View Controller (MVC) framework?
Model- stores and retrieves data, maintain state, observe change of state
View- renders model, user interaction side
Controller- respond to user input, instructs model to respond to user

### 3. Using the information given, complete the steps for creating a new view in a rails app by filling in the blanks:

  1. Create a route:

  code:
  ```
  get '/about' => 'statics#about'
  ```
  file: config/routes

  2. Create the __CONTROLLER__

  code:
  ```
  class __StaticsController < ApplicationController

  def about
    __render about_
  end
  ```

  file: __statics_controller.rb__

  3. Create the View

  code:

  ```
  <div>This is the About page!</div>
  ```

  file: __about.html.erb__


### 4. Look at these sets of Rails routes, they are an example of which principle/term that we touched on briefly in class? Find the term, and explain why it is important.
Create
Read
Update
Destroy
```
/users/       method="GET"     # :controller => 'users', :action => 'index'
/users/1      method="GET"     # :controller => 'users', :action => 'show'
/users/new    method="GET"     # :controller => 'users', :action => 'new'
/users/       method="POST"    # :controller => 'users', :action => 'create'
/users/1/edit method="GET"     # :controller => 'users', :action => 'edit'
/users/1      method="PUT"     # :controller => 'users', :action => 'update'
/users/1      method="DELETE"  # :controller => 'users', :action => 'destroy'
```

### 5. What is the public folder used for in Rails?
It's your favicon, error messages

### 6. Write a rails route for a controller called "main" and a page called "game" that takes in a parameter called "guess"
get '/game' => 'main#guess'

### 7. What are cookies for? How do they work? What is the difference between a session and a cookie?
Cookies are used for storing. They store key value pairs. Session data is stored on the server and cookies are stored on the clients browser.

### 8. In an html form, what does the "action" attribute tell you about the form?  How do you designate the HTTP verb for the form?
Action attribute is the URL. HTTP verb refers to the method.

### 9. Why would you use an instance variable in a rails controller?
Instance variable makes it available to the entire scope of the app.

### 10. Name two rails generator commands and what files they create:
rails g controller - creates controller
rails g model - creates table/database

### 11. There is a table called "squirrels". What SQL code would we write to print everything in the table?
SELECT * FROM squirrels
### 12. What is a foreign key? Where would you use it in a has many/belongs to relationship?
[Your Answer]
In SQL the foreign key is a field in one table the identifies a row in another talbe. Those two tables have one id in common.

[Googled Answer]
A FOREIGN KEY is a key used to link two tables together. It is a field (or collection of fields) in one table that refers to the PRIMARY KEY in another table.

### 13. Rails has a great community and lots of free tutorials to help you learn. Here is a list of some tutorials to choose from, choose one, do it, and then report back here at least one thing you learned. You can also use a different resource if you find one that you like better.
-In MVC the rails model is a ruby class that can add database records, you can find specific data, update that date, and remove it.

- https://www.tutorialspoint.com/ruby-on-rails/index.htm
- http://railsforzombies.org
- http://guides.rubyonrails.org/getting_started.html
