### Conceptual Exercise

Answer the following questions below:

- What is PostgreSQL?
  - PostgreSQL is a RDBMS or Relational Database Management System for SQL. 

- What is the difference between SQL and PostgreSQL?
  - SQL is the querying language, and PostgreSQL is the RDBMS that stores and manages the database. SQL is the language used to communicate with the PostgreSQL server to perform queries / make changes. 

- In `psql`, how do you connect to a database?
  - `$psql db_name`

- What is the difference between `HAVING` and `WHERE`?
  - `HAVING` is used to filter values from an existing `GROUP BY`
  - `WHERE` is used to filter results before grouping. 

- What is the difference between an `INNER` and `OUTER` join?
  - an `INNER` join grabs data from two tables and joins only data from both tables that match
  - an `OUTER` join grabs data from two tables, joins data that match, but also includes data from one table or the other that may not match (`LEFT` or `RIGHT` joins)

- What is the difference between a `LEFT OUTER` and `RIGHT OUTER` join?
  - a `LEFT OUTER` join, as mentioned above, takes the all matching and non-matching data from the table referenced in the `FROM` keyword
  - a `RIGHT OUTER` join takes all the matching and non-matching data from the table referenced after the `JOIN` keyword

- What is an ORM? What do they do?
  -An ORM (Object Relational Modeler) converts database tables into workable object-oriented classes that can be used in your code. 

- What are some differences between making HTTP requests using AJAX 
  and from the server side using a library like `requests`?
  - For `requests` on the server side:
    - Prevents same-origin issues when making requests from AJAX on the client-side.
    - It's easier to store and process data (Happens on one system and doesn't have to be sent back over. Server handles everything. No further JSON parsing required)
    - If you need a password or token to access an API, you won't be able to make the requests from AJAX unless each client has its own token. 
  - For AJAX requests on the client side:
    - Requests are fairly easy with AJAX libraries
    - Doesn't have to use server resources for making API calls
    - Has the potential of being much faster because the clients can talk directly to the API

- What is CSRF? What is the purpose of the CSRF token?
  - CSRF = Cross-site request forgery
  - It's when you can edit the form action on one site to point to another site. Without a CSRF token, there's no way to verify that any form information you receive truly came from forms you generated in your templates. CSRF checks a token sent with the form with the one generated on your server to verify that the information you're receiving is from a valid client source from your website, and not another website. 

- What is the purpose of `form.hidden_tag()`?
  - in WTForms, there are elements that are hidden/you can hide that you wouldn't typically want see in the form (Notably, the CSRF token field), but can involve other things if they aren't necessary in this particular form. 

  
