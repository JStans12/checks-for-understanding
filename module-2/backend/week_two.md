## Week Two - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!). 

Note: When you're done, submit a PR. 

1. At a high level, what is ActiveRecord? What does it do/allow you to do?
  - an ORM that helps to build databases and allows you to manipulate them like objects.
2. What kind of methods are `belongs_to`, and `has_many`? (i.e. class or instance) Give an example.
  - instance methods. you call them on a specific instance. Ed = Horse.first; Ed.stable; => stable object. This is made possible because a horse belongs_to a stable.
3. What do they allow you to do?
 - Find the stable that a horse belongs_to and the horses that a stable has_many of.
4. What's the difference between agile workflow and waterfall method?
  - Agile doesn't aim to have everything figured out before starting. It takes it one step at a time. Waterfall is the oposite.
5. What is the difference between `#new` and `#create`?
  - #new makes a new object. #create makes an object and saves it in the database.
6. At a basic level, what does cURL allow you to do?
  - send http requests from terminal
7. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.
  - Many to many. They will be joined through a students_teachers table that has columns for student_id and teacher_id
8. Define foreign key, primary key, and schema.
  - A foreign key points to the id column of another table. A primary key is in the ID column or another unique column. Schema is the outline of the entire database and acts as a map of table relationships.
9. Describe the relationship between a foreign key on one table and a primary key on another table.
  - The foreign key points to the primary key of another table. A horse has a foreign key called stable_id that is set to the ID of the stable it belongs to.
10. What are the parts of an HTTP response?
  - Status code, Headers and Body.
11. Describe some techniques to make our Sinatra code more DRY. Give an example of when you would use these techniques.
  - use a layout.erb so you dont need to write your header and footer in each template.


### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
  - Pluck is my single favorite. Give it column names and it returns an array of the row values. You can give it multiple arguments.
2. Name your three favorite ActiveRecord rake tasks and describe what they do.
  - nuke is a top secret rake task that i stole from Sal's .bash_profile. it does rake db:drop, create, migrate, test:prepare all in one.
4. What can you expect from a group as you begin working together? As you continue working together?
5. What two columns does `t.timestamps null: false` create in our database?
  - created_at, updated_at
6. What cURL flag can you use to send a `POST` request?
  - POST ??
7. What case does JSON (and JavaScript) use for multi-word variables?
  - camel
8. What case does Ruby use for multi-word variables?
  - snake
9. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
10. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
11. Give an example of when you might want to store information besides ids on a join table.
12. Describe and diagram the relationship between patients and doctors.
13. Describe and diagram the relationship between museums and original_paintings.
14. What are some examples of acceptable values for the parts of an HTTP response?
15. What types of output do we want to test when we test our controllers?
16. What could you see in your code that would make you think you might want to create a partial?
  - repetative forms like in create and update.
17. Why might you use a helper method?
  - if there is excessive logic in the controller. Methods other than the path methods.
