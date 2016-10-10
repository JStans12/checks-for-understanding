## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. List the five common HTTP verbs and what the purpose is of each verb.
  - GET - receive a request to view a page
  - POST - submit data to a website
  - PUT PATCH - update existing data
  - DELETE - delete data
2. What is Sinatra?
  - Framework for creating webapps with ruby
4. What is MVC?
  - Model View Controller is a way to organize a webapp.
5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
  - Sometimes convention is required by a gem/framework. Other times we just want others to understand.
6. What types of variables are accessible in our view templates without explicitly passing them?
  - instance variables
7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?
 - include @count in your controller in the method that calls index.erb
  
  ```ruby
  get '/horses' do
    erb :index
  end
  ```

8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed`?
 - between do and end add @name = 'Mr. Ed'
9. What's the purpose of ERB?
  - to embed ruby in html
10. Why do I need a development AND test database?
  - the test database needs to be torn down every time. you may want to hold data in the development database.
11. What's responsive design?
  - adjusting page layout to different resolutions and sizes
12. What is CRUD and why is it important?
  - create, read, update, destroy. the 4 main things we want to do to databases.
13. What does HTTP stand for? 
  - Hypertext transfer protocol
14. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
  - <% ruby %> wont appear on page. <%= ruby %> will appear on page
15. What's an ORM?
  - object relational mapper. allows us to treat database rows as objects.
16. What's the most commonly used ORM?
  - active record
17. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
  - CREATE
    - GET /new - view new record template
    - POST /thing - create new thing
  - READ
    - GET /index - view all things
    - GET /thing/:id - view specific thing
  - UPDATE
    - GET /edit/:id - view edit template
    - PUT /thing/:id - update thing
  - DELETE
    - DELETE /thing/:id - destroy
18. What's a migration? 
  - a record of how to create a database
19. When you create a migration, does it automatically modify your database?
  - no
20. How does a model relate to a database?
  - a model is like the outline for a table. it also holds methods to interact with that table.
