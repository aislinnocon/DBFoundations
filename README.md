# DBFoundations

SQL Views, Functions & Stored Procedures

Introduction: 
In this write up, I will discuss when I would utilize a SQL view, and the similarities and differences between Views, Functions, and Stored Procedures.

SQL View:
I would use a SQL View to create a layer of abstraction between the user and the database. This way if there are changes made to the database, it won’t necessarily mean that anything changes for the user. When I make a new table, I would make a base SQL View that will be used to be called upon by the user rather than the actual table itself. Additionally, I can deny public access to the original table, then allow public access only to the SQL View to further safeguard the table.

Views, Functions, and Stored Procedures:
1.	View: A View is a used to save Select Statements, typically more complex ones that would be tedious to retype. Views are incredibly useful in also safeguarding the original table and its data from interference from a user. Unlike a Function, parameters cannot be passed into a View. 
2.	Function: Functions can either return a whole table or just a singular value. Functions within SQl are similar to a View, but differ in their ability to take in parameters. Another difference with Functions, is that they can be used as an expression, something a View cannot do. 
3.	Stored Procedure: Like both, Views and Functions, Stored Procedures are a set of SQL statements that are named and can be called upon again.  

Summary:
Views are a way to create an abstraction layer between the database and the user to prevent changes from being made, both to the database and how the user interacts with the database. Stored Procedures, Views, and Functions, all share the commonality of being a set of SQL statements that is saved, and can be called upon later. Functions standout since parameters can be passed into Functions, and scalar Functions can be utilized as an expression. 
