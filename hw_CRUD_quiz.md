# CRUD Quiz

Use the solution to this afternoon's Property Tracker lab to answer the following questions. Please write your answers under each question, push the file to GitHub, and submit in the usual way.

## MVP Questions

In our Property Tracker application:

Q1. Where are we instantiating instances of the `Property` class?
# console.rb, lines 6, 15 & 24.

Q2. Where are we defining the SQL that enables us to save the ruby `Property` object into the database?
# property.rb, line 18.

Q3. In `console.rb`, which lines modify the database?
# lines 4, 13, 22, 31 & 33.

Q4. Why do we not define the id of a `Property` object at the point we instantiate it (‘new it up’)?
# To avoid having two (or more) instances with the same id which is set by the database.

Q5. Where and how do we assign the id (that is generated by the database) to the ruby `Property` object?
# property.rb, lines 29 & 32.

Q6. Why do we put a guard (an `if` clause) on the `@id` attribute in the constructor?
# To prevent errors when converting the @id to an integer (Nil can't be made an INT).

Q7. Why are some of the CRUD actions represented by instance methods, and others by class methods?
# The instance methods work on a specific record in the database which represents the "property", the class method does something else? 

Q8. What type of data structure is returned by calls to `db.exec_prepared()`? In the `save` method, how do we access the id from the returned data structure?
# a function and an array, by calling the id from the first record and storing it as an integer.

Q9. Why do we use prepared statements when performing database operations?
#To avoid SQL injection attacks.

## Extension Questions

Look at the `find_by_id` and `find_by_address` methods in the `Property` class.

Q10. What do they take in as their arguments?


Q11. What are their return values?
